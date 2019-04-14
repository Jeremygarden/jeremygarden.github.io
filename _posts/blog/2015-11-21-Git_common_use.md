---
layout: post
title: "Git common use"
author: me
excerpt: ""
categories: blog
tags: [Git, Coding]
modified:
image:
  feature: mushroom.jpg
  <!-- credit: WeGraphics -->
  <!-- creditlink: https://wegraphics.net/downloads/free-ultimate-blurred-background-pack/ -->
share: true
comments: true
---

Git is one of the beautiful things if you act as a dev on the stage.

I have nothing to say except love it.

But this post is coming across some frequently used commands. Just tagged as my notes for review.
![git daily workflow](https://1.bp.blogspot.com/--uNcah6YUSw/UZaB5xCzMNI/AAAAAAAAAhs/khSzRB0MIkc/s1600/git_everthing_is_local.png)

* git init - initialise (create) a repository
* git clone - copy an existing repository
* git branch - list, create or delete branches
* git checkout - checkout a branch, commit or file
* git add - add file contents to the index (staging area)
* git rm - Remove files from the working tree and from the index
* git commit - Record changes to the repository
* git log - Show commit logs
* git branch new_version # create a new branch of development  
* git checkout new_version # switch to the new branch  
* git merge new_version # merge the changes from new_version into the master branch  
* git pull /path/to/some_other_project new_version # pull changes from an existing git repository and merge them into a branch  
* git fetch /path/to/some_other_project master # pull changes from an existing repository without merging 

The [clear image](https://members.sange.fi/~atehwa/slides/git-slides.html) from Panu, his Git Training shows the basic and daily process if you need to modify, update, communicate between local working directory and remote repository.

Furthermore,
Git is a huge gem for team collaboration. Everyone has to touch it in order to working efficiently and effectively.

![git Dev Cycle](https://backlog.com/app/themes/backlog-child/assets/img/guides/git/collaboration/using_branches_002.png)

Here is the workflow model that demostrate the project releasing framework. There are also Centralized, Feature Branch, Forking and Merging. I keep this pic here for reminding me clearly when I think about adding or modify some feature on my projects. So more details have been nicely posted on the Atlassian website for you guys if you are interested.




### Reference links and useful tutorials:
[Code School 15 Mins Quick Try](https://try.github.io/levels/1/challenges/1)

[Atlassian official tutorials](https://www.atlassian.com/pt/git/workflows#!workflow-gitflow)

[My favorite one with awesome interactive effects](https://pcottle.github.io/learnGitBranching/)

You gotta check this out right now!