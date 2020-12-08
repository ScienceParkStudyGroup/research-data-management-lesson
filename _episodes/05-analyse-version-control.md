---
title: "Version control your analysis with git"
teaching: 45
exercises: 15 
questions:
- "What is version control?"
- "WHow can I be sure of the script and data I used to generate my manuscript figure?"
- "What are popular version control systems?"
objectives:
- "Understand the importance of version control for tracability of results."
- "Be able to display the differences between two (small) datasets or two workflows."
- "Be able to upload a dataset to one of the open-access repositories. "
keypoints:
- "Version control allows you to retrieve the complete history of your processed data and analytical workflows."
---

# 1. Table of contents

<!-- MarkdownTOC autolink="True" -->

- [1. Introduction](#1-introduction)
	- [1.1 What is version control?](#11-what-is-version-control)
	- [1.2 How is it valuable for my research and Research Data Management?](#12-how-is-it-valuable-for-my-research-and-research-data-management)
	- [1.3 What is the `git` software?](#13-what-is-the-git-software)
- [2. Version control your next publication](#2-version-control-your-next-publication)
	- [2.1 Exercise 1: keeping track of a figure.](#21-exercise-1-keeping-track-of-a-figure)
	- [2.2 Tracking a processed dataset](#22-tracking-a-processed-dataset)
- [3. Moving online](#3-moving-online)
	- [3.1 GitHub](#31-github)
	- [3.2 GitLab](#32-gitlab)
	- [3.3. BitBucket](#33-bitbucket)

<!-- /MarkdownTOC -->

# 1. Introduction

<img src="../img/04.research-data-cycle.png" width="600px">

## 1.1 What is version control?

## 1.2 How is it valuable for my research and Research Data Management?

## 1.3 What is the `git` software?

# 2. Version control your next publication

## 2.1 Exercise 1: keeping track of a figure.

Make a folder. Respect the previous folder structure and naming convention that you've choosen before.

Add a dataset (link)

Open RStudio and create a new script. Add a comment (using the \# sign followed by your comment.)

Open the Shell and navigate (`cd`) into the folder that you have created previously. 
Type `git init`

Type `git status`

Create a plot: 
  - read the data
  - make a back and white plot with ggplot. 
  - save your figure as a `.png`

Type `git status`

(untracked files)

`git add`
`git commit `

`git tree`


You are not so happy with this figure. You could perhaps add some color. 

`git add`
`git commit `

`git tree`


## 2.2 Tracking a processed dataset

Your figure is produced from a relatively small files (X megabytes). You have noticed that some numbers need to be corrected because this measurement was mixed up. 

	


# 3. Moving online 

## 3.1 GitHub
Provides hosting for software development and version control using Git.
Free for Open Source project. 

## 3.2 GitLab

## 3.3. BitBucket