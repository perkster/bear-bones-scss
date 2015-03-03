# BEAR-BONES.scss

This is a repository of the Sass files that accompany the bear bones WordPress theme (https://github.com/perkster/perkster-bear-bones). The theme is based on BEM methodology and does not use (much) semantic classes. Instead, utilizing the BEM (block, element, modifier) model, it is easy to switch up designs by just switching out one stylesheet. 

Over the years, I've come across some amazing frameworks, in particluar inuit.css by Harry Roberts. These files are based HEAVILY on his work but also on 320 and up by Andy Clark. I found myself constantly trying to get the two to play nicely and incorporate some of the great classes of each theme/framework, so I came up with my one and thus bear bones was born. Additionally, I have come across many other good frameworks like susy and purecss. So this framework will play nicely with other so you can pick and choose what you want to work with.

This css "framework" does not try to implement a bunch of styling objectives, instead it gives you the framework to put together a design of your own. 

Obviously, its meant to work with the Bear Bones theme and thus has things named in accordance with it. But since they are block based, you can apply many of the 


## File Structure ##

* scss/bear-bones/ 
* scss/plugins/
* scss/templates/
* scss/theme/
* scss/_bb-setup
* scss/_layout
* scss/_theme-style
* scss/_theme
* style.scss

### Bear Bones folder ###

This folder contains the "framework" and the vast majority of classes are placeholder classes. The "bb" prefix is used so it should play nice with other sass plugins. 

There is a bb_setup.scss file in the theme folder that has flags that you can turn on and off to make using bear bones easier. Of course, you're more than welcome to just add in whichever files you want into your project, too. 

Most of the files are pretty well documented including links to urls which the code comes from.

### Plugins ###

This folder holds scss plugins like include-media, inuit, susy, purecss, although the only plugins included in this are include-media as it is what is used for responsive design.

### Templates ###

This folder holds the blocks used for easy styling. Most files have a few variables at the top to assign things like colors, font variables, padding, margins, etc. 

### Theme ###

This is the folder that holds all the files that have the design elements.

* html - specific styling for html elements
* js - specific styling for js plugins
* objects - specific styling for objects such as nav, search, footer
* pages - specific styling for certain types of pages such as pages, posts, events
* plugins - since this is a WP theme, what WordPress website would be complete without plugins. Here is where you store the styling for specific plugins.
* style - the general style atributes such as brand, colors, buttons, typography
* woocommerce - WooCommerce is our preffered WordPress ecommerce solution (for now) and our theme comes WooCommerce ready. Styling for products, categories, etc. go here.

### Files ###

* bb-setup - Where you turn on flags for bear-bones modules. By default, modules are set to false.
* layout - Where the site layout structure is set.
* theme-style - loads up all of the style files rather than having to include them all on the main style.scss file
* theme - this is where you can include any css plugins, js plugins, templates and other theme specific style files.
* style - Files are loaded in this order: bb-setup, theme-style, bear-bones/bear-bones, plugins (include-media), theme