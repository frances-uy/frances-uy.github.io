---
layout: essay
type: essay
title: "Does My Code Really Work?"
# All dates must be YYYY-MM-DD format!
date: 2023-09-20
published: true
labels:
    - Coding Standards
    - ESLint
    - JavaScript
---

There’s no better feeling than your code finally running and working after spending hours on hundreds of lines of code. In my past computer science courses, I would have instinctively submitted my files right away. However after completing several more projects, it did not take long for me to realize that working code does not necessarily equate to good code.

What separates good code from bad code is __readability__. Code should not only produce expected results, but it must also be fairly easy for a fellow classmate, teacher, or colleague to read. Readability requires writing and presenting code in an easily written and read fashion. Readability can be established by __coding standards__, which are guidelines and best practices that are used to create consistent, high quality code.  

<div class="text-center"><img style="drop-shadow" src="../img/coding-standards-comic.png" alt="comic"></div>

## Coding Standards for Our Class

Coding standards will vary between classes or workplaces, but in this Software Engineering Class I am taking this Fall, we strictly follow the [AirBnB JavaScript Style Guide](https://github.com/airbnb/javascript). It has been adhered to for our weekly Workout of the Day (WOD) exercises. WODs are essentially timed coding challenges utilizing JavaScript, HTML, and CSS to solve given scenarios. Passing the WOD for the week requires its completion before a set time—otherwise it would be a hard fail. A critical part of the WOD is ensuring that we are following the coding standards for the class. To make it even easier for us to follow these coding standards, we use ESLint alongside the popular [IntelliJ IDEA Integrated Development Environment (IDE)](https://www.jetbrains.com/idea/). 

## What is ESLint?

ESLint is a downloadable linting utility for JavaScript that raises errors on parts of code that violate guidelines of the AirBnB JavaScript Style Guide. They have a handy [documentation](https://eslint.org/docs/latest/rules/) about all the errors you may encounter. It is widely used by top companies around the world, and is customizable for your own rules. In other words, you can take advantage of this free, open source tool to automate compliance with certain standards. The best part is that it catches them early on in the development process, while you’re coding.

## The ESLint Experience for WODs

When properly installed and enabled in IntelliJ, ESLint activates automatically every time a JavaScript file is opened. Setting up ESLint by configuring my Editor settings in IntelliJ was a bit of a hassle at first. It was a series of one-time steps of updating the default code style, defining the JavaScript version as ECMAScript 6+, and disabling non-ESLint IntelliJ inspections. However as we continue to do more WODs, I’m starting to get used to it and like it. It raises red error warnings if there is a guideline violation, and displays a green checkmark if there are none. Descriptions of the errors detected in the current file and quick-fixes for them are available from the editor and from the Problems tool window. Non-ESLint IntelliJ inspections are disabled.

<div class="text-center"><img width="1000" src="../img/eslint-error.png"></div>

Entering the command `meteor npm run lint` in the terminal is a guaranteed way to see if you violated ESLint standards without having to shift through all your JavaScript files. Here is an example of the violation above:

```
(base) michelleuy@MacBook-Pro-28 app % meteor npm run lint

> meteor-application-template-react@ lint /Users/michelleuy/Desktop/github/digits/app
> eslint --quiet --ext .jsx --ext .js ./imports && eslint --quiet --ext .js ./tests


/Users/michelleuy/Desktop/github/digits/app/imports/api/contact/Contacts.js
  36:1  error  Too many blank lines at the end of file. Max of 0 allowed 
```

Most of my errors so far were minor, such as inconsistent spacing in parentheses, too many spaces at the end of the program, and even double quotes instead of single quotes. However, I noticed it was much easier to debug my functions if I did not receive the expected output, because my code was organized. I saved time during our WODs because I did not have to spend precious minutes looking for very small mistakes (like a missing curly brace) that would prevent the program from running in general. The green checkmark of no errors that ESLint provides is also good personal reassurance for the final check through I do before actually submitting the WOD. Just to make sure that everything looks good format-wise.

## Coding Standards for the Real World

The biggest nightmare in software engineering would be an inability to read your own code or someone else's code. Software engineering has a lot of team-based work, meaning code and behavior will be frequently passed around. It would be a pain to have to completely redo a project just because the current code was not maintainable for other developers through coding standards. When we complete our end of the project, we want to commit _quality, error free code_ to the GitHub repository. It needs to be readable in order to be reproducible, in case you wanted to use it as a future template or make changes on the existing application.

The moral of the story: follow your organization's coding standards. It may take extra time reading through documentation and implementing it. However you could waste more time reading code with no structure whatsoever. With practice and patience, coding style should become second nature. It is an advantage to get to focus on the many features of the coding language and your powerful capabilities, without worrying about our formatting.