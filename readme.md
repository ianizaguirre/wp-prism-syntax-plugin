### Prism Syntax Highlighter Plugin For WordPress

Original library developed by - [Lea Verou](https://github.com/PrismJS/prism)

Original Plugin developed by - [ankurk91](https://github.com/ankurk91/wp-prism-js)

### Description

Prism is a lightweight, extensible syntax highlighter, built with modern web standards in mind.
This WP plugin lets you control and use this awesome library in to your WordPress site.

---

> **[Original WP Plugin link](https://wordpress.org/plugins/ank-prism-for-wp/) the latest working copy**

---

# Changes Made

## Color Scheme - Added Cobalt2

* I added my own theme based on WesBos Cobalt2 Color Scheme

### How it was done

(1) File Path: _lib / themes_

* Now drag and drop a new CSS theme.

(2) File Path: _inc / class-util.php_

* Around line 23, you should see `$list = array`

* Now create a new array item, for example:

`7 => array('name' => 'Cobalt2WesBos', 'url' => $baseUrl . 'prism-cobalt2wesbos', 'file' => 'prism-cobalt2wesbos'),`

Save your changes, and thats it. Your new color scheme should now appear as a Plugin setting option.

---

## Updated a few Plugin CSS files

I Changed these CSS files to better match the new Cobalt2 Color Scheme

### Path 1

Path: plugins / prism-show-language.css

### Path 2

Path: plugins / prism-copy-to-clipboard.css

---

## Added New Plugin

The current version of this WordPress plugin lacks some newly added features/plugins that the non-WordPress Prism Git Repository has added recently.

### Added - Unescaped Markup Plugin

Date: 2-8-18

I added the Unescaped markup plugin

(1) Path: lib / plugins

* I added the unescaped-markup **[min.js file & .css file](https://github.com/PrismJS/prism/tree/gh-pages/plugins/unescaped-markup)** from the Prism repository, to the "plugins" folder.

(2) Path: inc / class-util.php

* Around line 42, you should see `$list = array`

* After list item "16", add:

`17 => array('name' => 'Unescaped Markup', 'url' => $baseUrl . 'unescaped-markup/', 'file' => 'prism-unescaped-markup', 'need_css' => 1),`

Save your changes, and thats it. The Unescaped markup plugin should now appear as a Plugin option, under the "Select plugins" section.
