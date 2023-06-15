# GWD Resources

This repository contains webpage templates and HTML/CSS code snippets for use in a future outreach event.

## Template Instructions

HTML/CSS webpage templates are stored in the `templates` folder. Each webpage template contains the following elements:

1. Boilerplate HTML webpage code (`<!DOCTYPE html> declaration tags`, `<head>` tags, etc)
2. HTML elements (`<p>' elements, etc)
3. Inline CSS styling (`<style>` elements in the `<head>` tags)

To use a pre-made HTML/CSS webpage template, do one of the following:
1. Copy the content of the `.html` file and paste into your personal `.html` file.
2. Download the `.html` file and upload it to your personal workspace.

## Snippet Instructions

HTML/CSS code snippets are stored in the `snippets` folder. Each code snippet may contain the following elements:

1. Boilerplate HTML webpage code (`<!DOCTYPE html>` declaration tags, `<head>` tags, etc)
2. HTML elements (`<div>' elements, etc)
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

## Resources

Resources for webpages (images, linked HTML pages, etc) are stored in the `resource` folder. Any HTML element that requires an image or a linked HTML page uses the `resource` folder. 

## Acknowledgements

This repository of HTML and CSS elements is built upon the lessons and examples provided by W3Schools (www.w3schools.com). I would like to acknowledge their valuable resources and educational material, which have greatly contributed to the development of this project.
