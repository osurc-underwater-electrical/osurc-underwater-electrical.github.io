# Site Format

The general format for the documentation is 

    - Overview

        - General Info 

    - Current Design

        - Getting Started (links to current year's design, and must be changed manually each year)

    - Other Crud

## Why this format?

The primary of goal of any documenation is to explain something.  In this case, we want to explain the design for the electrical components of the undwater ROV created for the OSU Robotics Underwater team.

It is also important to understand how the design has changed over time.  Consequently, it makes sense to split the documentation by year.  Additionally, if the design changes significantly between years---as it has in past, and will in the future---then each year is free to have its documents structured to best convey design intent.

If there are only a few changes between years, it should be a simple matter to copy files into a new folder for the new year and add the changes there.

## Writing new pages

This site is built with docsify.  It was chosen because it can be simply installed, and is an easy, lightweight way to organize files into a webiste.  Visit the docsify [website](https://docsify.js.org/#/) to learn in detail about how it can be used to write documentation.

Basically, when a new page needs to be written, one only needs to create a new Markdown file (ends in .md) somwhere in the `docs` folder and docsify will automatically format it into a webpage and serve it up for viewing.

## Customizing Web Structure

Customization of the website is performed in the `index.html` file, and lies in the website's root directory.  All links made to other Markdown files are relative to the location of the `index.html` file.

### The Coverpage

Docsify responds to a number of special files.  Most of them are prefixed with an underscore, `_`.  The coverpage is described by `_coverpage.md`, and must be set in the `index.html` so that docsify with render it with `coverpage: true`.  To make it the only part of the homepage, set `onlyCover: true`.

### The Side Bar

The side bar is the thing on the left-hand side of the page.  Sidebars are described in `_sidebar.md` files.  For the current site format to work, each folder that contains each year's documentation (or the documenation for this maintenance stuff) needs its own `_sidebar.md` file.  Then `loadSidebar = True` must be set in `index.html`.  That way the sidebar relevant to a folder's documentation will be shown, instead of the main sidebar in the root directory.

Basically, whenever more documentation is created that would make sense to gateher into a folder, a `_sidebar.md` must be included in that folder, and the sidebar file must contain a link that returns it to the previous directory.

### The Navigation Bar

The custom navigation bar, the thing in the top right corner of this web page, is described in `_navbar.md` and is set in `index.html` with `loadNavbar = True`.  Curretnly, the nav bar contains links to each years documentation---its a link to the archives.  Its not an entirely necessary component, as a the root sidebar could also be configured to point to archived documentation, but the nav bar was simple and rather elegant.  Additionally, it can be accessed from any web page.

### The Search Bar

The search bar can be used as an aid to finding something in the documenation.  It doesn't seem to work that well, or it takes some time to register changes to the documentation, so items that definitely exist don't always appear in the search.  Still, it may be of some use, so it has been added.


