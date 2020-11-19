---
title: "Project and file management"
teaching: 30
exercises: 0
questions:
- "How can I consistently organise my folder during my research project?"
- "Are there any good consistent way to name files?"
- "What should I avoid when it comes to file naming?"
- "How can I add simple explanations about a folder content?"
- "Are there specific tips regarding publications and scripts (version control)?"
objectives:
- ""
- ""
keypoints:
- "."
---

## Table of Contents


<!-- MarkdownTOC autolink="True" -->

- [Making a consistent project folder structure](#making-a-consistent-project-folder-structure)
    - [Experimental results](#experimental-results)
- [File naming conventions](#file-naming-conventions)
    - [Consistency and convention](#consistency-and-convention)
    - [Good practices](#good-practices)
    - [Problematic characters](#problematic-characters)
- [Hosting publication and scripts on a git hosting service \(e.g. GitHub\)](#hosting-publication-and-scripts-on-a-git-hosting-service-eg-github)
    - [Host your publication on a social network of code \(e.g. GitHub\)](#host-your-publication-on-a-social-network-of-code-eg-github)
    - [A concrete example with GitHub](#a-concrete-example-with-github)
        - [Set up a paper repository](#set-up-a-paper-repository)
    - [Display contributions and paper history](#display-contributions-and-paper-history)
- [Resources](#resources)
    - [Blog post](#blog-post)
    - [Tutorials](#tutorials)

<!-- /MarkdownTOC -->


# Making a consistent project folder structure


Use a number in front of your folder (`01.admin/`) so that, even if the name of the folder is changed, the folder stays at the same location. 

## Experimental results

Raw data need a README.txt file in the same folder with some human-readable explanation. This `README.txt` file should for instance contain:
1. your comments from your laboratory notebook: "This experiment will determine whether a loss-of-function of the gene _EATME_ of lettuce (_Lactuca sativa_) has an effect on the fresh weight of first stage caterpillar larvae from the _Manduca sexta_ (tobacco moth) species after 14 days. etc.".
2. A dictionnary for the column names in your spreadsheets (e.g. "weight: weight of the larvae in mg") to h 
3. 


# File naming conventions

## Consistency and convention

When starting a new research project (e.g. your PhD), one of the most profitable RDM practice is to implement a consistent and understandable folder and file anming structure. 

This consistent scheme will be applied to the same type of data for example. Think about one experiment where you collect samples from a field site and you will want to collect information on:
- The date of the result collection. 
- The person that collected the sample. 

## Good practices

__Date formatting__ is perhaps both the most important and easiest to set. If you use the __YYYYMMDD__ format then your files will be easily sorted by date.   
__Avoid special characters in file names__: avoid special characters and spaces when separating the different elements of your file name, do not use spaces or characters like "?@{[<>"" etc. Some software programs (e.g. R) do not work well with file names with these characters. You can use dashes and underscores instead.


## Problematic characters
Some cha

# Hosting publication and scripts on a git hosting service (e.g. GitHub)

We often think of a scientific publication as the holy grail of one scientist's work. While this is particularly true in a given academic environment where scientific prestige and reputation are directly related to the journal and citations you have, the _pièce de résistance_ (main content) lies in the collection of files underlying your research publication:  
- Manuscript: a piece of formatted text.
- Figures: image files (e.g. `.png` or `.jpeg`), vector graphic files (`.svg`, `.pdf`, `.eps`) formats, etc. 
- Supplementary information files
- Raw and/or processed data underlying the figures and scientific conclusions. 
- Data-processing code files (e.g. R script for a particular figure).  

## Host your publication on a social network of code (e.g. GitHub)
- Data underlying figures and conclusions all hosted online openly.
- Add scripts underlying each figures in the same online repository.  
- Make it public at the end of the publication process. 
- The data to figure process is made more open and can be added to the publication itself.


- If data are too big to be hosted on GitHub (> 100Mb), provide a persistent identifier (doi, link) to the datasets. 
on GitHub

## A concrete example with GitHub

### Set up a paper repository

In version control hosting service jargon, a "repository" is a place to put your precious publication-related data. This is obviously the first step. This is what it could look like in the end:

<img src="../images/02-paper-on-github.png" width="80%" alt="Hosting a publication on GitHub">

You can add a [tag](https://www.atlassian.com/git/tutorials/inspecting-a-repository/git-tag) to a certain version of the paper such as "version submitted to Nature journal on December 4, 2020". This would point to a specific commit number making it easy to trace back what has been submitted, when and who contributed at the time to the paper.  

## Display contributions and paper history

In combination with `git`, GitHub will act as a "time machine" where all changes to files and figures are recorded. This makes it easy to undo things if necessary or to point to a specific change in history.

<img src="../images/02-full-commit-history.png" width="80%" alt="commit history">

GitHub helps to list the number of contributions of each author. It can also be a way to see who contributed the most to a publication for instance in a rationale way.

> ## Discussion
> How does this version 

<img src="../images/02-contributions.png" width="80%" alt="GitHub view of contributors in a given repository">

As you can see, two authors have contributed relatively equally to this publication as can be seen from the number of commits. Yet, one commit can be rather small (changing one file and committing) or be the result from a more extensive work (creating a figure, adding the related script, etc.). This depends on the "commit behaviour" of the person in this case. 


> ## Discussion
> What do you think are some pros and cons for hosting your publication on a git hosting service? Can you think of short-term and long-term benefits for your research?
{: .discussion} 

# Resources

## Blog post
- A nice blog post on how git and GitHub are particularly well suited for scientific project and file management: [link](https://grasshoppermouse.github.io/2019/07/12/should-scientific-publishing-move-to-github-and-friends/).
- List of academic publications hosted on GitHub: [https://github.com/topics/academic-publication](https://github.com/topics/academic-publication)

## Tutorials
- [The Software Carpentry Lesson on version control with git and GitHub](https://swcarpentry.github.io/git-novice/). 




{% include links.md %}
