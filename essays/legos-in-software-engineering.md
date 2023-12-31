---
layout: essay
type: essay
title: "Where Creativity Meets Structure"
# All dates must be YYYY-MM-DD format!
date: 2023-11-29
published: true
labels:
    - Design Patterns
    - Software Engineering
---
## The Building Bricks of Software Engineering

Just like a child’s fascination with a brand new LEGO set, at a high-level, a software engineer experiences a similar excitement when piecing together a project using design patterns. Each LEGO brick represents a component in your software. It varies in size, shape, and functionality. Understanding its purpose is crucial in building a complete, functional structure. Design patterns are these fundamental building blocks. Like following the step-by-step instruction manual at the bottom of the box, there is usually a standardized approach to solving common problems in software design patterns.

[LEGO Certified Professionals](https://www.lego.com/en-us/aboutus/lego-certified-professionals) passionately curate these sets out of thousands of tiny pieces. They envisioned a model for a customer to build in a certain way. They figured out how to transform numerous 3 x 6 blocks into a miniature Eiffel Tower or sports car. There was a process involved in between the placement of the first block and the final model.

Design patterns, in essence, are not just solutions to common problems. They are methodologies, honed in by experts in the Software Engineering field that have years of experience and knowledge. Design patterns are intended for other developers to be able to encounter a problem of that kind, and have a template to solve it. These design patterns provide a standardized approach to solving common problems in software design, much like how LEGO bricks are used to construct various models.

<div align="center">
 <img src="https://github.com/frances-uy/frances-uy.github.io/blob/main/img/lego.jpeg?raw=true" width="500px"/>
</div>

## Following the Instructions: Learning the Basics

In the Software Engineering class (ICS 314) that I am currently taking, the majority of the code I wrote, including our [final project](https://askusits.site/), was based on this [meteor-react-template](https://ics-software-engineering.github.io/meteor-application-template-react/), created by one of the instructors. It gave us a head start on Meteor development, deployment, and boilerplate code to implement basic page display, navigation, forms, roles, and collection manipulation.

We are also introduced to these four most popular design patterns, akin to the various themes and difficulty of LEGO sets:

- **Creational Patterns (The Foundational Blocks)**
    - These are the base plates and foundation bricks in a LEGO set. They deal with object creation in a manner appropriate to the situation. The **Singleton Pattern** is responsible for managing global configurations and states.

- **Structural Patterns (Building the Framework)**
    - This is the interconnectedness of the blocks, ensuring that code is organized into logical, interconnected blocks. **MVC (Model-View-Controller) Pattern** ensures that the application is maintainable and scalable.

- **Behavioral Patterns (Bringing the Model to Life)**
    - The **Observer Pattern** is used for managing reactive updates, akin to adding dynamic, moving parts to a LEGO creation. This pattern allows various components of the application to communicate efficiently, reflecting changes across the system seamlessly.








## The Timeless Nature of LEGOs

LEGOs are reused and valued for their ability to be reconfigured into new models. The design patterns that were utilized in the template were the Creation and Structural Patterns. This way the application was separated into three interconnected components. Just like when you first open a LEGO set, the bricks are separated into smaller 3-5 plastic bags so it is easier to follow the instruction manual.

The creation of our ArticlesCollection in our [final project](https://askusits.site/) was one example of a Singleton Pattern instance. This is a instance of which other parts of the system have global access to it. This access to the collection is needed in order to carry out various tasks in the application, such as providing related source links and generating the best possible answer. It is feasible that only one instance of the ArticlesCollection exists throughout the lifetime of the application.

Anyone can use a statement like this to make their own collection. Originally in the template this was used to make a `StuffsCollection`, but in our final project we were dealing with University of Hawaii’s Information Technology (IT) articles. These articles are critical as our final project is an AI Chatbot that answered IT related questions.

````
export const Articles = new ArticlesCollection();
````

## Build On!

Unless you’re an extreme LEGO fanatic, there is still a lot to learn in the field. Design patterns offer a structured approach to creativity and problem solving. Each piece based on a pattern plays a critical role in both the our tangible and virtual creations. There really is no "final piece" that can ultimately complete the build in Software Engineering. Seasoned professionals in this field continue to learn, and build on their builds each time.
