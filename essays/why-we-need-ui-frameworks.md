---
layout: essay
type: essay
title: "UI-nifying Design: Why do We Need UI Frameworks?"
# All dates must be YYYY-MM-DD format!
date: 2023-10-04
published: true
---
## What is UI and Why Do We Need It?

UI (User-Interface) Design is a quintessential part of Software Engineering. It is the point of contact between humans and computers. The elements of UI include navigational elements (search fields and back arrows), input controls (buttons, checkboxes, and text fields), informational components (progress bars), and containers (organization of content). 

Our goal as software engineers should not only be to develop programs that work, but also provide a way to make sure that the intended user can actually _use_ it. Other than just looking nice, we want it to be accessible and appealing to the user.

Website layouts are the main type of UI that I have been experimenting with lately in our Software Engineering class. We have been able to create simple websites with raw, basic HTML and CSS, such as this Browser History website. Here is the result:

<img src="https://github.com/frances-uy/frances-uy.github.io/blob/6faf88d735efc5520188e7d4251cf3ab5689309f/img/browser-history-website.png?raw=true" alt="Browser History Website" style="box-shadow: 10px 10px 10px gray; width:700px;"/>

The code was very simple. I displayed the information through header, paragraph, and image tags. Here is a snippet of a section of it:

    <body>
        <h2>Introduction</h2>
        <p>The first web browser was invented in 1990 by Tim Berners-Lee. It was called WorldWideWeb (no spaces) and was 
        later renamed Nexus. In 1993, Marc Andreesen created a browser that was easy to use and install with the release of 
        Mosaic (later Netscape), "the world's first popular browser", which made the World Wide Web system easy to use and 
        more accessible to the average person. Andreesen's browser sparked the internet boom of the 1990s. These are the two 
        major milestones in the history of the Web.

          The wars put the Web in the hands of millions of ordinary PC users, but showed how commercialization of the Web 
        could stymie standards efforts. Both Microsoft and Netscape liberally incorporated proprietary extensions to HTML in 
        their products, and tried to gain an edge by product differentiation, leading to the acceptance of the Cascading 
        Style Sheets proposed by Hakon Wium Lie over Netscape's JavaScript Style Sheets (JSSS) by W3C.
        </p>
    </body>


The reality is that no modern website for a business or company would actually look like this. This example is functional in simply displaying information, but it does not allow the user to interact with it. If I needed to, for example, add a blue button or area for customer inquiry, it would take an extensive amount of HTML and CSS. It is possible. But it would not be an efficient use of time for multi page websites or fancy elements.

## Why UI Frameworks Are Useful

UI Frameworks are collections of pre-built design elements, components, and libraries that can be linked in your .html file and be referenced in your code. Some of the most well-known UI frameworks include React, Angular, jQuery, Semantic-UI, etc. However, we have been introduced to the UI framework [Bootstrap](https://getbootstrap.com/docs/5.3/getting-started/introduction/) so far. Their documentation answers any design implementation challenge you may have.

## My Experience with Bootstrap

The biggest obstacle for me so far across my projects was horizontally and vertically centering text or images. Using raw HTML and CSS I had to create a class and manually set margins and padding for the top, bottom, left, and right. This was how I was centering the text in paragraph elements at first in my .css file:

    p {
        font-family: 'Open Sans', 'sans-serif';
        text-align: center;
        top-margin: '10px';
        bottom-margin: '10px';
        left-margin: '50px';
        right-margin: '50px';
      }

<img src="https://github.com/frances-uy/frances-uy.github.io/blob/6faf88d735efc5520188e7d4251cf3ab5689309f/img/centering-html.png?raw=true" alt="Browser History Website" style="box-shadow: 10px 10px 10px gray; width:700px;"/>

That is a lot of lines to customize. With Bootstrap, I was able to use the classes ‘text-center’ and ‘justify-content-center’ to do the same centering task in a fraction of the steps, like this for example.

    <div class="justify-content-center text-center">
         <h2 class="textcenter">Now accepting reservations for St Patrick's Day</h2>
         <h2 class="textcenter">Please call 808-531-0422 for reservations</h2>
         <h2 class="textcenter">St Patrick's Day To-Go Orders can be ordered</h2>
         <h2 class="textcenter">on our website menu.</h2>
         </div>

<img src="https://github.com/frances-uy/frances-uy.github.io/blob/6faf88d735efc5520188e7d4251cf3ab5689309f/img/centering-bootstrap.png?raw=true" alt="Browser History Website" style="box-shadow: 10px 10px 10px gray; width:700px;"/>         
One neat thing that Bootstrap also provides is a library of 1300+ high-quality icons. For example if you want to include social media icons to a navigation bar, all you need to do is copy a link that looks like this and paste it where needed (usually I place them inside a <ul></ul> element).

    <i class="bi bi-instagram p-3"></i>
    <i class="bi bi-facebook p-3"></i>
    <i class="bi bi-twitter p-3"></i>

<img src="https://github.com/frances-uy/frances-uy.github.io/blob/6faf88d735efc5520188e7d4251cf3ab5689309f/img/bootstrap-icon-navbar.png?raw=true" alt="Browser History Website" style="box-shadow: 10px 10px 10px gray; width:700px;"/> 

Although importing the Bootstrap Icon Library is another step to have to do, it is significantly more efficient than doing it with raw HTML and CSS. Looking at the latter route, not only would you have to find a high-quality image from the internet yourself, but you would need to center it and pad it manually. 

I found that Bootstrap made recreating websites in class so much faster and allowed my code to be more readable through simplicity. What could go wrong?

## Beginner’s Warning

I ought to share a fair warning that UI Frameworks only work as we become familiar with its syntax and capabilities. Although Bootstrap is a toolkit for JavaScript, HTML, and CSS (languages I'm already familiar with) I felt like Bootstrap 5 was a completely new language at first. Using a UI Framework is supposed to make developing easy, but it felt slow at first. It is well worth spending time to understand Bootstrap's rules and documentation. They have a handy search bar that can help you find what you need fast. That way you could avoid unreadable code or frustration when the line doesn’t work.

At some points I experienced the complete opposite, wherein Bootstrap 5 felt too easy. In the beginning I felt that Bootstrap limited the exploration of CSS. When using UI Frameworks, you can take the look for granted and not know what goes on behind the scenes. This is something to be aware of if competency with CSS is your goal. I did have prior knowledge with CSS, so applying the Bootstrap framework was a good way to reinforce how classes worked and how to override them for styles. Having CSS knowledge is important for manipulating fonts, font colors, backgrounds, and more. I found it simpler to implement these choices in CSS instead of using Bootstrap. Knowing how CSS code works also allows you to easily find out the reason why Bootstrap elements may not work when you apply them.

I believe that UI Frameworks like Bootstrap will never make your life easier by doing the coding work for you. It is a more standardized way of UI Design, but it can get complicated for a beginner. Knowing how to use it gives you an advantage as a Software Engineer, since almost every website you see uses UI Frameworks. 

