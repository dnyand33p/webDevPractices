# Getting Started with HTML

## What is HTML?

* A "markup" language, where we "mark" text (with elements) to add structure & meaning to it. Such as to say which text part of a document is a list, heading, paragraph, image, table or a form (to collect user input) etc.

``` html
  I Love H <sub> 2 </sub> 0
```

> I Love H<sub>2</sub>0

* Used by search engines (to help users find relevant information), screen readers (to navigate the page), browser (to generate DOM - which is used to style and manipulate element with css and html respectively).

## HTML, CSS, JavaScript - 3 Partners in Crime.

* Set of rules written in these 3 languages will decide:
  +  *What a web page will contain?*

     * Text, images, links, videos, invisible trackers, loggers, cookie handlers etc.

  +  *How it will look?* 

     *  How the elements will jump in and out when we scroll down.
     *  What will they do when we hover over them -- buttons changing color, slide show pauses on mouse hover etc.

  +  What elements will do on interacting with them?

     *  Clicking a button with mic icon will open a mic hardware for listening -> listen and convert to text -> write in an empty text-field.

*  All the experience we as a user get from a web page are decided by there threes with guidelines of UI/UX -- to map the tasks user want to perform, with these set of micro-interactions. 
*  We could use libraries to avoid re-writing common things (react, bootstrap, jquery), communicate with hardwares of client machine with Browser APIs (Zoom Meetings -- To stream data - voice/video calls, To store login info with different approaches -- cookies, JWT), really today's web interactions can be anything you can think of.

> As a construction analogy -while construction a building - *beams, column structure, bricks are like HTML*. Plaster, *color of a wall is styling as in* CSS and turing on shower with knob, opening door etc. are like *behaviors - JavaScript*

## HTML Element Anatomy

* Web page -- when stored as file is a collection of nested html elements, which are made up of tags, attributes and text.

``` html 
  <openingTab attribute> content </closingTag>

``` 

* Tags comes with different names(p, header etc.)to mark the meaning of content. Most elements are made up of opening tag and closing tag but some have opening tags only.
* Attributes gives different types of additional info about the element.

```html
  <img src="/img/namaste.jpg">
```

## HTML Boilerplate

* Please check the [lifeOfBenjamin.html](lifeOfBenjamin.html) , read the comments.
* **Boilerplate** is basic skeleton, from which we start authoring code file further i.e common starting point.

   + In VS Code type "!" and hit tab to generate a HTML Boilerplate. (from within a .html file).
 

``` html
  <!doctype html>
  <html lang="eng">

  <head>
      <title> I will be displayed in list of search result, as a tab new in browser and while bookmarking </title>
      <meta description="I will be shown below the title in search result list">
  </head>

  <body>
      I will hold visible element & some scripts to load after rendering whole page.
  </body>
```

* Thise boilerplate tells browsers and search engines which html version it is using **(<!doctype html>)**, where to find more info about this page -- in  **\<head>** tag and it's elements to be displayed - in **<body>** element --> further we *nest* more elements inside these *head* and *body*. 

## Life of an HTML Page

* User requests a page (by putting in URL in browser).
* Server sees the request and create the HTML page on fly or sends the one already stored in file system

    >* Template is like raw structure of page - a blueprint with thing that won't change and a *place holder* for things that will.
    >* We populate these *place holders* with customized data (according to location - for different languages, user, time or data from database) by running some logic (with monolith or serverless functions) -- and then an HTML page is created and served to requester.
    

# Concept of DOM.

* DOM Tree is like a web page in running. Each html elements have a corresponding node -at the hierarchy. 

  + When we author a page we have nested html elements -> when browser loads and renders the page, it create a **DOM** - Document Object Model to dynamically manipulate elements (to animate, add, remote, change on event)
  + HTML Elements are attached to document object in a web browser for create a DOM.
  + Elements have relationships between them such as child, parent, siblings, ancestors etc. which are used to conditionally select and element (aka. *node* is DOM)

## Common HTML Elements.

* **Headings** are six of them - from h1 to h6. Each page should have only one h1 and they should be nested in order.

* 

##  How to author an HTML Page.

 My thoughts on authoring a website. -- here on a web page only.

* Decide which info you want to be shown on page -> then gather textual data, illustrations, images etc.
* Create a folder for webpage, put resources (images, videos, stylesheets, scripts etc) in it.
* Put all the textual info in Body tag.
* Mark up textual data in relevant HTML elements.
* Make a links to navigate on the same page as well as to jump to other pages.
* Add attributes to link to all  resources (.css, .js, media)
