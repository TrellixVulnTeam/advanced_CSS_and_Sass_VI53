# advanced_CSS_and_Sass


Feature Section 
-----------------------------------
Edit the layout using the CSS grid 
Skew the section 7 degress;
Move the margin top by -15rem to connet the top left corner with the about section


Card section 
-----------------------------------
Use perspective define at the parent element
    The lower the value the more dramatic the flip effect 

Card flip effect
    set backside rotate to 180 degree as default setting 
    Set the backface-visibility property 

The background blend mode to blend the background image and picture together without using photoshop to do so;


Use the box-decoration-break to edit the subtitles for each card especially when the text is wrapped to show the outline layout to align one another.

Stories Section
-----------------------------------
Make text flow around shapes with shape-outside and float;

Apply a filter to images;

Create a background video to covering an entire section; 

Use the <video>HTML element;

Use the object-fit property to adjust the video ratios to fit with the section;


Booking section 
-----------------------------------
linear-gradient to divide the background image to two views.

::-webkit-place-holder selector to change the content of the placeholder text

:focus and :focus:invalid to verify the input types by different color of the box bottom line.

Footer section
-----------------------------------
General page footer setting, copyright and other information.


Bonus - pop up function with only CSS
-----------------------------------
Use ::target pseudo-class, to implement the pop up;

Use display:table at the parent element and display:table-cell in the child element to create boxes with equal height.

Use vertical-align: middle, to set the content in the table cell in the position of middle in the cell.

Use hyphens to automatically hyphenate words


Make responsive page
-- Adapt the page to different screen sizes
-----------------------------------
Use Sass mixin to write all media queries;
    
Use @content,  to adding settings into the original @mixin argument;
    
Use @if statement to work with @mixin to include all breakpoints in to one argument;

Taking advantage of Chrome DevTool for responsive design.

Doing the responsive image in HTML
1. Density switching
2. Art direction
Use srcset attribute width description and size attribute of the <img> element to allow the browser to decide the best image to download.


Building Process with NPM Scripts
-----------------------------------
   <code> "watch:sass": "node-sass sass/main.scss css/style.css -w",
    "devserver":"live-server",
    "start":"npm-run-all --parallel devserver watch:sass",
    "compile:sass": "node-sass sass/main.scss css/style.comp.css",
    "concat:css": "concat -o css/style.concat.css css/icon-font.css css/style.comp.css",
    "build:css": "npm-run-all compile:sass concat:css "</code>