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
#### Step 2 - Populate it with a readme
#### Step 3 - Find a new theme you like
#### Step 4 - Replace your existing files with the theme's files
#### Step 5 - Modify ad infinitum

### Creating a repository:
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



