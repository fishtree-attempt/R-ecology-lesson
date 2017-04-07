---
layout: lesson
title: Data carpentry: R for data analysis and visualization of Ecological Data
keywords: ["R", "subset", "data.frame", "read.csv", "dplyr", "ggplot2"]
---

This is an introduction to R designed for participants with no programming
experience. These lessons can be taught in 3/4 of a day (6 hours). They start
with some basic information about syntax for the R programming language, the
RStudio interface, and move through to specific programming tasks, such as
importing CSV files, the structure of data.frame objects in R, dealing with
categorical variables (i.e. factors), basic data manipulation (adding/removing
rows and columns), and finishing with calculating summary statistics and a
brief introduction to plotting.

## Prerequisites
>
> * Having R and RStudio installed (though see the first lesson, [Before we start](00-before-we-start.html)
for installation instructions)

## Topics

* [Before we start](00-before-we-start.html)
* [Introduction to R](01-intro-to-R.html)
* [Starting with data](02-starting-with-data.html)
* [Aggregating and analyzing data with dplyr](03-dplyr.html)
* [Data visualization with ggplot2](04-visualization-ggplot2.html)
* [R and Databases](05-R-and-databases.html)

## Organization of the repository

The lessons are written in Rmarkdown format. A Makefile generates the
corresponding html page for each lesson by running rmarkdown from within R. In
the process, rmarkdown creates an intermediate markdown file. These are removed
by the Makefile to avoid clutter.

The Makefile also generates a "code handout" file that is intended to be
distributed to the participants. This file includes some of the examples used
during teaching and the titles of the section. It provides a guide that the
participants can fill in as the lesson progresses. Participants can also copy
and paste from this file to avoids typos for more complex examples. Each lesson
generates a code handout file, and the files produced are then concatenated to
create a single file and the intermediate files are deleted. To be included in
the code handout file, a code chunk in the Rmarkdown lesson file needs to have
the arguments `purl=TRUE`.
