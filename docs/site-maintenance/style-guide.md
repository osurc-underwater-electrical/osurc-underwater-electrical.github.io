# Style Guide

If you are a documentation maintainer, or just want to write docs directly, this page will serve as a reference to maintain consistent style among the pages.
Most of these styles are derived from the Markdown [guide](https://www.markdownguide.org/basic-syntax/).<br>
Please refer to it for more in depth information and best practices.

There is also a cheat sheet available [here](https://www.markdownguide.org/cheat-sheet/).

*P.S. these suggestions are just recommendations.  A future doc maintainer should feel free to change the style if they want.*<br>
*P.P.S. this page will make more sense if the raw markdown is [read](https://raw.githubusercontent.com/osurcue/osurcue.github.io/master/docs/site-maintenance/style-guide.md)*

## Lists

Use the - (hyphen) when writing unordered lists.  Ident with a tab to create a sublist. Items of differnt hierarchy should not be separated by a blank line, but items or different hierarchy should.

For instance, do this:

- Top Hierarchy
- Same Hierarchy

    - Sublist item
    - Same hierachy as sub list

- Top hierarchy again

Not this:

- Top Hierarchy
- Same Hierarchy
    - Sublist item (should have preceding blank line)

    - Same hierachy as sub list (should **not** have preceding blank line)
- Top hierarchy again (should have preceding blank line)

## Bold and Italics

Use one asterisk ( * ) for italics, like this: *this is in italics*

Do not use the underscore character.

---

Use two asterisks ( ** ) for bold, like this: **this is in bold**

Do not use the underscore character.


## Images

The images are stored on a CDN to reduce the size of repository but still provide a central location for image sources.

Use an HTML `<img>` tag to include an image from there like this (changing the src of course):

<img src="https://ik.imagekit.io/kjbx6tb5231/default-image.jpg" alt="arch way" style="width:100px;height:100px">

It is also possible to use markdown format to include an image, but HTML will provide more customization an freedom when placing and sizing images.  The HTML `<img>` tag is the preferred format. 


## Paragraphs and line breaks

Put one whole blank line between paragraphs like

this

Use the  HTML `<br>` tag to perform a line break li<br>
ke this

## Everything Else

Go read the Basic Syntax Markdown [guide](https://www.markdownguide.org/basic-syntax/).  It's short and can be referenced when writing things in the documentation.<br>
It's a well written guide and includes many of the best practices included here.