# What should be core

support for beautiful table, expressively described
support for all fonts? utf8 by default of course.
support for insertion of pictures

# Fundamental concepts

- Layers
- boxes and glue (the Tex way of describing how to work with words)
- doc test

# Separation of layout and content

the way I see things now is for each project you have two files, a .rl (for riplatex) file that is a description of the layout and a .content file that is a content and might be compatible with any .rl files.

There is a mismatch if an `object` mentioned in the content file is not defined in the .rl file

# 2 fundamental classes

Boxes and Glue.

An object is either some kind of box (it takes some place)
Or some kind of glue (it glues some box or other glue object together and end up taking some place).

# Must have library

- International (support for different languages (english, french etc)) that describe hyphenation, and warn when there is an orthography mistake. 
- Tikz_like drawing and more

# Hooks

The capacity of executing code at the start of each page? end of document?

# Anchors

Immutable points that inform you were you are in the layout.

A few global : ThisPage (the number of the page, the margins of the page); This document (number of pages);

Scoped local ones: lastElement(position, indentation,custom anchor)

Anchor after : Every `object` must define the `after` anchor, it describe where you should put an object after that one.

Anchor center, left , right, bottom_left, bottom_right, etc should be automatically derived for each object.

## Custom Anchors

Imagine you are defining a function to draw a beautiful circle, you can specify a `my_label` anchor.
When someone wants to draw your circle and add a label, they might do something like:
(remember nothing has been decided about the syntax or such)
```
circle = draw_circle(RED,SIZE::CM::16)
circle.my_label = draw_text("This is a beautiful label",SIZE::MEDIUM)
```

# Errors