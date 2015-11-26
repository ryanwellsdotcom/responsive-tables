##jquery.responsive-tables

A lightweight jQuery plugin  that allows table markup to become fully responsive. It provides a clean list  view via devices with small screens. It can work for multiple tables on a  single page, as well as with tables that contain various combinations of merged  cells. Best of all, it uses pure CSS for the rendering. 

###How to use

include the <em>responsive-tables.css</em> in your page within the &lt;head&gt;&lt;/head&gt; tags

Include the <em>jquery.responsive-tables.js</em> in your page after <a href="http://jquery.com/download/" target="_blank">jQuery</a>

invoke the plugin within your custom scripts file: 
```javascript
$(document).ready(function() {
    $.responsiveTables();    
});    
```
Ensure that tables are marked up using the &lt;thead&gt;&lt;/thead&gt; and &lt;tbody&gt;&lt;/tbody&gt; tags
Add the class 'respond' to the &lt;table&gt; tag of the chosen table(s):
```html
<table class="respond">
    <caption>Example</caption>
    <thead>
        ...
```
###customizations 

Within the <em>responsive-tables.css</em> style sheet, modifying the values of the 'top' and 'left' properties will change the perceived table heading padding at the &quot;mobile&quot; view. This will enable consitancy between the table heading and table data padding:
```css
table.respond td:before { 
    /* top/left values mimics padding */
    top: 8px;/* mimics padding top */
    left: 6px;/* mimics padding left */
```

within the <em>responsive-tables.css</em> style sheet, change the media query breakpoint as needed:
```css
@media only screen and (max-width: 800px) 
```

###Author

Ryan Wells: [@ryanwellsdotcom][twitter]

###License

Licensed under [MIT][mit]. Enjoy.

[twitter]: https://twitter.com/ryanwellsdotcom
[mit]: http://www.opensource.org/licenses/mit-license.php
[jquery]: http://jquery.com/