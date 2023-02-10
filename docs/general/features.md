---
title: Features
weight: 10
---

Like many people, I don't really enjoy writing documentation, so I tried to take most of the pain out of it. This site will do a lot of work around structuring the documentation that is written and making it look pretty.

## Automatic section/menu structure

On the left, you can see the section menu. This menu is constructed using the directory structure of the documentation that was pulled into the site generator. Under the hood, this is using Hugo (which has some [relevant documentation](https://gohugo.io/content-management/sections/) about how to structure content sections). Currently, this site only understands two levels of sections: each top level project is a section, and then each of the headings that you see in the left menu are also sections. They cannot be nested deeper than that in the current site.

There is a small amount of manual work that may need to be done to get things to show up in the right order. In the `_index.md` for any given section, you can set a `weight` value in the front matter. This will be used for determining the order that pages show up in the menu. You can also set a `weight` value on each individual page if you want to control the order within a section.

## Automatic table of contents

If you're using a wide enough screen, you'll see that there is also a table of contents to the right of this text. The table of contents is generated from the heading structure in the document. It generally does the right thing most of the time, but it really helps if the text headings don't skip levels in either direction. It's probably a good idea to avoid doing that anyway.

Note that the table of contents is only added when there are multiple headings in the document. Otherwise, the column won't show up at all.

## GitHub links

Each top-level project section can have a `github` attribute, which should be a link to the project repository. Setting this value makes the GitHub icon in the top right of the screen show up for the project. That value is also used to build the "leave some feedback" links at the bottom of each inner page. Setting the `github` attribute is optional, but recommended -- it is much easier for people to contribute to documentation when they know where the source files are at.
