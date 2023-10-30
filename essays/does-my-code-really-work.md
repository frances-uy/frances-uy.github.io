---
layout: essay
type: essay
title: "Does My Code Really Work?"
# All dates must be YYYY-MM-DD format!
date: 2023-09-20
published: true
---

There’s no better feeling than your code finally running and working after spending hours on hundreds of lines of code. In my past computer science courses, I would have instinctively submitted my files right away. However after completing several more projects, I have realized  working code does not necessarily equate to good code.

What separates good code from bad code is __readability__. Code should not only produce expected results, but it must also be fairly easy for a fellow classmate, teacher, or colleague to read. Readability requires writing and presenting code in an easily written and read fashion. Readability can be established by __coding standards__, which are guidelines and best practices that are used to create consistent, high quality code.  

## Coding Standards for Our Class

Coding standards will vary between classes or workplaces, but in this Software Engineering Class I am taking this Fall, we strictly follow the [AirBnB JavaScript Style Guide](https://github.com/airbnb/javascript). It has been adhered to for our weekly Workout of the Day (WOD) exercises. WODs are essentially timed coding challenges utilizing JavaScript, HTML, and CSS to solve given scenarios. Passing the WOD for the week requires its completion before a set time—otherwise it would be a hard fail. A critical part of the WOD is ensuring that we are following the coding standards for the class. To make it even easier for us to follow these coding standards, we use ESLint alongside the popular [IntelliJ IDEA Integrated Development Environment (IDE)](https://www.jetbrains.com/idea/). 

## What is ESLint?

ESLint is a downloadable linting utility for JavaScript that raises errors on parts of code that violate guidelines of the AirBnB JavaScript Style Guide. They have a handy [documentation](https://eslint.org/docs/latest/rules/) about all the errors you may encounter. It is widely used by top companies around the world, and is customizable for your own rules. In other words, you can take advantage of this free, open source tool to automate compliance with certain standards. The best part is that it catches them early on in the development process, while you’re coding.

## The ESLint Experience for WODs

When properly installed and enabled in IntelliJ, ESLint activates automatically every time a JavaScript file is opened. Setting up ESLint by configuring my Editor settings in IntelliJ was a bit of a hassle at first. It was a series of one-time steps of updating the default code style, defining the JavaScript verison as ECMAScript 6+, and disabling non-ESLint IntelliJ inspections. However as we continue to do more WODs, I’m starting to get used to it and like it. It raises red error warnings if there is a guideline violation, and displays a green checkmark if there are none. Descriptions of the errors detected in the current file and quick-fixes for them are available from the editor and from the Problems tool window. Non-ESLint IntelliJ inspections are disabled

Most of my errors so far were minor, such as inconsistent spacing in parentheses, too many spaces at the end of the program, and even double quotes instead of single quotes. However, I noticed it was much easier to debug my functions if I did not receive the expected output, because my code was organized. I saved time during our WODs because I did not have to spend precious minutes looking for very small mistakes (like a missing curly brace) that would prevent the program from running in general. The green checkmark of no errors that ESLint provides is also good personal reassurance for the final check through I do before actually submitting the WOD. Just to make sure that everything looks good format-wise.

Thinking ahead, following the coding standards for this class throughout the semester will make it easier to post neat, informative repositories of code from projects to Github. Reading code is essentially what Github users do for the most part, so it must be readable in order for them to read it or provide feedback. 

Not being able to read your own code at all must be addressed. It is common to spend a lot of work on a program, just to look at it either feeling a bit confused or completely overwhelmed. It’s avoidable by taking a moment to pause, go over the documentation for ESLint or coding standards, and utilize them as you code. With practice and patience, coding style should become second nature. It is an advantage to get to focus on the many features of JavaScript without worrying about our formatting. 
