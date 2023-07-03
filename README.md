# GWD Resources

This repository contains webpage templates and HTML/CSS code snippets for use in a future outreach event.

# Template Instructions

HTML/CSS webpage templates are stored in the `templates` folder. Each webpage template contains the following elements:

1. A HTML document (`<!DOCTYPE html>` tag, `<head>` tag, etc)
2. a CSS stylesheet (`h1 {color: red}` selector, etc)

To use a pre-made HTML/CSS webpage template, do one of the following:
1. Download the template's folder and upload it to your personal workspace.
2. Copy the content of the `.html` file and paste into your personal `.html` file. Then, copy the content of the `.css` file and paste it into your personal `.css` file.
     - If you do this and your HTML document styling is not working, [see the issue here](#i-copied-the-html-and-css-files-into-my-workspace-but-the-html-page-isnt-styled)

# Snippet Instructions

HTML/CSS code snippets are stored in the `snippets` folder. Each code snippet may contain the following elements:

1. Boilerplate HTML webpage code (`<!DOCTYPE html>` declaration tags, `<head>` tags, etc)
2. HTML elements (`<div>` tags, `<p>` tags, etc)
3. Inline CSS styling (`<style>` elements in the `<head>` tags)
**NOTE:** some HTML/CSS elements are in their own folders. These elements require other HTML/CSS webpages to work properly.  

To use the **HTML** elements, simply copy the HTML element and paste into your webpage.

**NOTE:** the HTML element may use inline CSS styling. If they do, they use _class_ selection to select specific HTML elements to style based on their class name. The HTML element will look like this:

```html
<h1 class="CLASS_NAME">My Heading</h1>
```

The inline CSS styling is stored in the `<style>` element, like this:

```html
<head>
  <style>

    /* HTML_ELEMENT */
    p {
      color: green;
    }

    /* HTML_ELEMENT . CLASS_NAME */
    h1.type1 {
      background-color: red;
    }

    /* .CLASS_NAME */
    .type2 {
      background-color: blue;
    }

    /* .CLASS_NAME <...HTML_ELEMENTS> */
    
    .type3 a, li {
      color: pink;
    }

  </style>
</head>
```

If the HTML element uses inline **CSS** styling, do one of the following:

- Copy the CSS styling in the `<style>` element into your personal webpage `<style>` element.
- Copy the CSS styling in the `<style>` element into your personal `.css` file.
     - If you do this and the styling is not working, [see the issue here](#i-copied-a-html-code-snippet-into-my-html-file-that-had-styling-but-its-no-longer-styled)

# Resources

Resources for webpages (images, linked HTML pages, etc) are stored in the `resource` folder. Any HTML element that requires an image or a linked HTML page uses the `resource` folder. 

# Common Issues

### _I copied the `.html` and `.css` files into my workspace, but the HTML page isn't styled._

By default, all `.html` files expect a stylesheet called `styles.css`. It is declared in each `.html` file's `<head>` tag:

```html
  ...
  <head>
    ...
    <link rel="stylesheet" type="text/css" href="styles.css" />
    ...
  </head>
  ...
```

To fix this, do either of the following:
1. Rename your CSS stylesheet to `styles.css`
2. Change the `href` attribute's value from `styles.css` to your `.css` file name.

### _I copied a **HTML** code snippet into my `.html` file that had styling, but its no longer styled_

Code snippets such as `buttons.html`, `headers.html`, etc use **CSS** *inline styling* like this:

```html
  ...
  <head>
    ...
    <styles>
      h1.type2 {
        background-color: tomato;
        color: wheat;
        box-shadow: 2px 2px 4px black;
      }
    </styles>
    ...
  </head>
  ...
```

Each **CSS** in-line selector selects an HTML element based on the element's **tag** and *class* like this: **tag**.*class*.

The name tells the program that this styling should **only** apply to HTML elements of type **tag** of class *class*.

To fix this, do the following:
1. Include the **CSS** styling in either your `.css` file or your `<style>` element in your `.html` file.
2. Assign the **HTML** element a *class* name matching the *class* name on the **CSS** styling, like this:
```html
  <h1 class="type2"> My Header </h1>
```
 


# Acknowledgements

This repository of HTML and CSS elements is built upon the lessons and examples provided by W3Schools (www.w3schools.com). I would like to acknowledge their valuable resources and educational material, which have greatly contributed to the development of this project.
