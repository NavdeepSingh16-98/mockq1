# mockq1

The CSS position property is used to set position for an element. it is also used to place an element behind another and also useful for scripted animation effect.

You can position an element using the top, bottom, left and right properties. These properties can be used only after position property is set first. A position element's computed position property is relative, absolute, fixed or sticky.

Let's have a look at following CSS positioning:

- CSS Static Positioning
- CSS Fixed Positioning
- CSS Relative Positioning
- CSS Absolute Positioning

## CSS Static Positioning
This is a by default position for HTML elements. It always positions an element according to the normal flow of the page. It is not affected by the top, bottom, left and right properties.

## CSS Fixed Positioning
The fixed positioning property helps to put the text fixed on the browser. This fixed test is positioned relative to the browser window, and doesn't move even you scroll the window.
```
<!DOCTYPE html>  
<html>  
<head>  
<style>  
p.pos_fixed {  
    position: fixed;  
    top: 50px;  
    right: 5px;  
    color: blue;  
}  
</style>  
</head>  
<body>  
  
<p>Some text...</p><p>Some text...</p><p>Some text...</p><p>........</p><p>.... ...</p  
><p>........</p><p>........</p><p>........</p><p>........</p>  
<p>........ </p><p>........</p><p>........</p><p>........</p><p>........</p>  
<p>........</p><p>........</p><p>Some text...</p><p>Some text...</p><p>Some text...</p>  
<p class="pos_fixed">This is the fix positioned text.</p>  
</body>  
</html> 
``` 

## CSS Relative Positioning
The relative positioning property is used to set the element relative to its normal position.


```
<!DOCTYPE html>  
<html>  
<head>  
<style>  
h2.pos_left {  
    position: relative;  
    left: -30px;  
}  
h2.pos_right {  
    position: relative;  
    left: 30px;  
}  
</style>  
</head>  
<body>  
<h2>This is a heading with no position</h2>  
<h2 class="pos_left">This heading is positioned left according to its normal position</h2>  
<h2 class="pos_right">This heading is positioned right according to its normal position</h2>  
<p>The style "left:-30px" subtracts 30 pixels from the element's original left position.</p>  
<p>The style "left:30px" adds 30 pixels to the element's original left position.</p>  
</body>  
</html>  
```

## CSS Absolute Positioning
The absolute positioning is used to position an element relative to the first parent element that has a position other than static. If no such element is found, the containing block is HTML.

With the absolute positioning, you can place an element anywhere on a page.


```
<!DOCTYPE html>  
<html>  
<head>  
<style>  
h2 {  
    position: absolute;  
    left: 150px;  
    top: 250px;  
}  
</style>  
</head>  
<body>  
<h2>This heading has an absolute position</h2>  
<p> The heading below is placed 150px from the left and 250px from the top of the page.</p>  
</body>  
</html>

```