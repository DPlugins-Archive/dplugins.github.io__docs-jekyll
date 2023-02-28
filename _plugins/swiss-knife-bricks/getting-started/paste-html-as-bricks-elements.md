---
order: 1
description: Winden is a Tailwind CSS integration for WordPress page builders.
title: Paste HTML as Bricks elements
---

# Paste HTML as Bricks elements

Revolutionary feature for bricks that will allow you to create entire website page or template with just couple of clicks. Copy entire page. Paste into bricks. Connect framework or add your classes system and you are up and running. 

## Enable the feature

This feature is disabled by the default.
Check `Paste HTML` and save changes.

## Before we get started

1. Be sure that website is https
	 
2. If you are pasting inline SVG elements be sure to enable "Code Execution" in Bricks Builder
	![](../img/code-execution.png)
	
	
## Usage 

You can copy any HTML from:
1. Code editor
2. Browser
3. Or Clipboard 

Into Bricks editor and it will be converted as Bricks element(s).

Once you copy HTML code use Right Click > Paste HTML or press "Down Arrow inside Clipboard" icon in the topbar. 

![](../img/paste-html-icon.png)

![](../img/paste-html-right-click.png)

### What will be converted

- All html elements 
	-  h1, h2, h3, h4, h5, h6
	-  p, link, buttons
	-  div, span
	-  images, svg (as img element, you will need to manually transfer image file to the media library)
	-  inline svg (will be added as code block as that is the closes that bricks have atm)
	-  classes will be attached to the elements

### What will not be converted	

Classes values. We are converting Classes values into Bricks. We are attacing classes names to the elements. 

## First time Usage 

Every time you use paste feature for the first time or some website or you clear the cache allow clipboard dialog box will be promted. Allow the feature or you will not be able to use it. 