---
order: 1
description: Winden is a Tailwind CSS integration for WordPress page builders.
title: Scripts Manager
---

## Enable the feature

This feature is disabled by the default.
Check Emable Scripts Manger and save changes.

![](../../img/sc_manager_1.png)

## Enable files upload

For self-hosting scripts, we use WordPress media uploaded and save scripts inside the media upload folder. WordPress does not allow .js and .css file types to be uploaded by default. That is why you must check "Allow CSS/JS Uploads." If you use scripts from CDN, you will not need this option enabled. 

## Add new script

Navigate to the Swiss Knife `Bricks > Scripts Manager` and press "+ Add New Script"

![](../../img/sc_manager_2.png)

## Scripts Configuration

![](../../img/sc_manager_3.png)

### Script Name

To make it easier to recognize, choose a unique and descriptive name. 
![](../../img/sc_manager_registered_scripts.png)

### Script Type

Script types you can upload are CSS Files (.css) or JavaScript Files (.js)
Select the script type from the Script Type dropdown menu.

### Location

Scripts and Styles can be sent to two locations. 
- Website header
- Website foooter (right before closing body tag)

For the best pratices we recoment sending .css to the header and .js to the footer.

### Include Type

The `wp_register_script()` function is used to register a new script with WordPress. This function does not actually include the script in the site, but rather creates a reference to it. By registering the script, WordPress keeps track of the script's dependencies, version number, and other information that can be used later when the script is actually enqueued.

The `wp_enqueue_script()` function is used to actually include a registered script in the site. This function adds the script to the page's HTML header or footer, depending on how it is called, and sets it to load in the correct order with other scripts on the page.

#### Add Script or Style on every page or post
Use **Enqueue Script**.

#### Add Script or Style on selected page or post
Use **Register Script**. With this option script will be prepared but not added on the page. On the page you want to display it you need to paste `wp_enqueue_script('gsap');` to the code block.

![](../../img/copy.png)

![](../../img/code_block.png)

In this case GSAP will be loaded on pages where you have code blocks with `<?php wp_enqueue_script('gsap'); ?>`			

### Frontend only

Working with animations that move or hide elements is difficult. For this reason, we introduced only the Frontend. Styles and scripts will only be loaded on the front end of the website and will not be accessible inside the Bricks Builder.


### Upload file or paste cdn link


