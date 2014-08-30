---
title: Solidarity Map
layout: interactive
permalink: solidarity/
body_id: solidarity
---

<!-- The StoryMap container can go anywhere on the page. Be sure to 
    specify a width and height.  The width can be absolute (in pixels) or 
    relative (in percentage), but the height must be an absolute value.  
    Of course, you can specify width and height with CSS instead -->
<div id="mapdiv" style="width: 100%; height: 600px;"></div> 

<!-- Your script tags should be placed before the closing body tag. -->
<link rel="stylesheet" href="http://cdn.knightlab.com/libs/storymapjs/latest/css/storymap.css">
<script type="text/javascript" src="http://cdn.knightlab.com/libs/storymapjs/latest/js/storymap-min.js"></script>

<script>
// storymap_data can be an URL or a Javascript object
var storymap_data = 'https://6ec89bf6e47c922a6b7e24eeeda2e1b88b28d0c9.googledrive.com/host/0B5TTgpc7dScaQW5KZ2dTMUJOOGM/published.json'; 

// certain settings must be passed within a separate options object
var storymap_options = {};

var storymap = new VCO.StoryMap('mapdiv', storymap_data, storymap_options);
window.onresize = function(event) {
    storymap.updateDisplay(); // this isn't automatic
}          
</script>
