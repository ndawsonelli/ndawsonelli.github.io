---
layout: post
title:  "Github Pages Tutorial"
date:   2017-12-13 8:00:00
img: github_pages.jpg
description: A demo blog post about modifying Jekyll themes!
---

## Modifying a Jekyll Theme to fit your needs
### There are several steps. In order, they are:
#### Step 1 - Create a github.io repository
#### Step 2 - Find a new theme you like
#### Step 3 - Replace your existing files with the theme's files
#### Step 4 - Modify ad infinitum
#### Step 5 - Troubleshooting tips

### Creating a Repository:
To create a repository, go to [github](github.com) and create a new repository.  This can be done from the main page, once you're logged in, and 
select the "New Repository" button.  

Then, name your repository, as per the image below, and type whatever you'd like into the README:
![image1](/assets/img/git_setup_2.PNG)

Once your repository is created, make a new folder somewhere on your computer and clone the repository to it.
This can be done using the following commands:
```
git init
git remote add origin httpw://github.com/<your_github_username>/<your_repository_name>.github.io.git
git pull -u origin master
```
### Finding a Theme
Head over to [Jekyll-Themes](http://jekyllthemes.org/) and start scrolling through them. If you find one you like, check out the demo!
This theme is called [Fresh](http://jekyllthemes.org/themes/fresh/)

### Download the Theme
Select the Download button, unzip the file, and paste it into your newly created folder.
Then, run the following commands. Feel free to change the commit message to whatever you like - the more descriptive, the better!
```
git add .
git commit -m "updating theme"
git push -u origin master
```

Next, head on over to your Github Pages home page!
If you're lucky, it'll look like this:
![img_3](/assets/img/git_setup_3.PNG)

If you're not, it'll look like this:
![img_4](/assets/img/git_setup_4.PNG)

Now, we're on to the final stage - modification and troubleshooting!

### Troubleshooting and Modification

In order to fix the above error, we need to modify the file that controls a lot of the features of the website - config.yaml
`Yaml` is a language that is similar to `Markdown` that usually interpreted by an engine and used for high-level modifications.

In this instance, the problem is with `baseurl` - the default baseurl doesn't match up with the other files which are created
by the jekyll engine.  To fix it, all we have to do is set the baseurl to "":
![img_5](/assets/img/git_setup_5.PNG)

While we're in there, we might as well modify the name and title as well.  These may have different effects depending upon 
their implementation, but generally the title changes the text at the top of the web page, located in the tab.




