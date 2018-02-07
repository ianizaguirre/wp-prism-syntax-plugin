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

* I added my own theme based on WesBos Cobalt2 Color Scheme

## How it was done

(1) Go to:
lib / themes

* now drag and drop a new css theme.

(2) Go to:
inc / class-util.php

* on line 23, you should see `$list = array`

Make a new array item, for example:
`7 => array('name' => 'Cobalt2WesBos', 'url' => $baseUrl . 'prism-cobalt2wesbos', 'file' => 'prism-cobalt2wesbos'),`

Save, and thats it. Your new color scheme should now appear as a plugin setting option.
