# Praetexo User Guide

## Table of Contents
- [Breakpoints](#breakpoints)
- [Containers](#containers)
- [Grid](#grid)
- [Navbar](#navbar)

## Breakpoints

Breakpoints are specific widths that are used to determine how a responsive layout works across devices.

Like many other CSS frameworks, Praetexo uses breakpoints representative of a set of common device sizes and viewports. These breakpoints allow the use of containers with widths that are a multiple of 12.

The breakpoints are as follows:
- Extra Small (< 576px)
- Small (576px - 767px)
- Medium (768px - 991px)
- Large (992px - 1199px)
- Extra Large (1200px - 1399px)
- Extra extra large (> 1400px)

## Containers

Containers are simple building blocks that contain content within a given device or viewport. Containers are responsible for padding and aligning content.

You can create a container by adding the <code>container</code> class to a div.

```html
<div class="container"></div>
```

## Grid

The grid system consists of rows and columns. Each row contains 12 columns. It is possible to create columns that span more than one column. 

Columns are specified using a span value. For a single column you use the <code>col-1</code> class. For a column that spans the entire row you use the <code>col-12</code> class, this is a column that spans across 12 columns - the default number of columns within a row.

To create a row with 3 equal columns you need to create divs using the <code>col-4</code> class (remember 12 / 3 = 4). For example:

```html
<div class="container">
    <div class="row">
        <div class="col-4">1</div>
        <div class="col-4">2</div>
        <div class="col-4">3</div>
    </div>
</div>
```

On Small and Extra Small devices / viewports, columns will be stacked vertically.

## Navbar

A navbar is a navigation header found on most websites. It contains the website title and a set of navigation links. On Small and Extra Small devices / viewports  the navigation is displayed as a hamburger menu that opens up a list of navigation items. On larger views it is simply a set of navigation links displayed next to each other with a space between them.

The navbar makes use of a hidden checkbox to toggle the list of navigation links for the hamburger menu. This eliminates the need for JavaScript.

The hamburger "icon" is a pure css icon and is drawn using three empty <code>span</code> elements.

Here is an example navbar:

```html
<nav>
    <a class="page-title" href="#">Site Name</a>
    <label for="menu" tabindex="0">
        <span></span>
        <span></span>
        <span></span>
    </label>
    <input id="menu" type="checkbox" />
    <ul>
        <li><a href="#">Mastodon</a></li>
        <li><a href="#">Twitter</a></li>
        <li><a href="#">Github</a></li>
    </ul>
</nav>
```