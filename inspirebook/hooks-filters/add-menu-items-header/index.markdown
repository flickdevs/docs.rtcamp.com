---
title: Add menu items in header
---

You can customize header with the help of hooks.

![header-menu](http://docs.rtcamp.com/wp-content/uploads/2014/11/header-menu.png)


## Add menu items in header:


`function test_nav_menu() {
echo 'Menu content';
}`
`add_action( 'rtp_hook_within_header', 'test_nav_menu' );`


## Remove menu items from slide panel:


`function rtp_remove_parent_hooks() {
remove_action( 'rtp_hook_end_slide_panel', 'inspirebook_theme_primary_nav_menu' );
}`
`add_action( 'init', 'rtp_remove_parent_hooks' );`
