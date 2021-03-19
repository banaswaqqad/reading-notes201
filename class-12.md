# Basic usage of canvas

This looks a lot like the  element, the only difference is that it doesn’t have the src and alt attributes. The element has only two attributes - width and height. These are both optional and can also be set using DOM properties. When no width and height attributes are specified, the canvas will initially be 300 pixels wide and 150 pixels high. The element can be sized arbitrarily by CSS, but during rendering the image is scaled to fit its layout size. (If your renderings seem distorted, try specifying your width and height attributes explicitly in the attributes, and not with CSS.)

The id attribute isn’t specific to the element but is one of the default HTML attributes which can be applied to (almost) every HTML element (like class for instance). It’s always a good idea to supply an id because this makes it much easier to identify it in our script.

The element can be styled just like any normal image (margin, border, background, etc). These rules however don’t affect the actual drawing on the canvas. We’ll see how this is done later in this tutorial. When no styling rules are applied to the canvas it will initially be fully transparent.

Fallback content Because the element is still relatively new, we need a means of providing fallback content when a browser doesn’t support the element.

This is very straightforward: we just provide alternative content inside the canvas element. Browsers which don’t support will ignore the container and render the fallback content inside it. Browsers which do support will ignore the content inside the container, and just render the canvas normally.

# Drawing shapes with canvas
Browsers give us several ways to display graphics. The simplest way is to use styles to position and color regular DOM elements. This can get you quite far, as the game in the previous chapter showed. By adding partially transparent background images to the nodes, we can make them look exactly the way we want. It is even possible to rotate or skew nodes with the transform style.

But we’d be using the DOM for something that it wasn’t originally designed for. Some tasks, such as drawing a line between arbitrary points, are extremely awkward to do with regular HTML elements.

There are two alternatives. The first is DOM-based but utilizes Scalable Vector Graphics (SVG), rather than HTML. Think of SVG as a document-markup dialect that focuses on shapes rather than text. You can embed an SVG document directly in an HTML document or include it with an  tag


 
 # Colors
Up until now we have only seen methods of the drawing context. If we want to apply colors to a shape, there are two important properties we can use: fillStyle and strokeStyle.

fillStyle = color
Sets the style used when filling shapes.
strokeStyle = color
Sets the style for shapes' outlines.
Color is a string representing a CSS `<color>`, a gradient object, or a pattern object. We'll look at gradient and pattern objects later. By default, the stroke and fill color are set to black (CSS color value #000000).



The valid strings you can enter should, according to the specification, be CSS `<color>` values.

# Transparency
In addition to drawing opaque shapes to the canvas, we can also draw semi-transparent (or translucent) shapes. This is done by either setting the globalAlpha property or by assigning a semi-transparent color to the stroke and/or fill style.

globalAlpha = transparencyValue

Applies the specified transparency value to all future shapes drawn on the canvas. The value must be between 0.0 (fully transparent) to 1.0 (fully opaque). This value is 1.0 (fully opaque) by default.

The globalAlpha property can be useful if you want to draw a lot of shapes on the canvas with similar transparency, but otherwise it's generally more useful to set the transparency on individual shapes when setting their colors.

Because the strokeStyle and fillStyle properties accept CSS rgba color values, we can use the following notation to assign a transparent color to them.



**The rgba() function**
 is similar to the rgb() function but it has one extra parameter. The last parameter sets the transparency value of this particular color. The valid range is again between 0.0 (fully transparent) and 1.0 (fully opaque).

 (Links to an external site.)Line styles
There are several properties which allow us to style lines.

lineWidth = value
Sets the width of lines drawn in the future.
lineCap = type
Sets the appearance of the ends of lines.
lineJoin = type
Sets the appearance of the "corners" where lines meet.
miterLimit = value
Establishes a limit on the miter when two lines join at a sharp angle, to let you control how thick the junction becomes.
getLineDash()
Returns the current line dash pattern array containing an even number of non-negative numbers.
setLineDash(segments)
Sets the current line dash pattern.
lineDashOffset = value
Specifies where to start a dash array on a line.
 (Links to an external site.)Gradients
Just like any normal drawing program, we can fill and stroke shapes using linear and radial gradients. We create a CanvasGradient object by using one of the following methods. We can then assign this object to the fillStyle or strokeStyle properties.

**createLinearGradient(x1, y1, x2, y2)**
Creates a linear gradient object with a starting point of (x1, y1) and an end point of (x2, y2).
createRadialGradient(x1, y1, r1, x2, y2, r2)
Creates a radial gradient. The parameters represent two circles, one with its center at (x1, y1) and a radius of r1, and the other with its center at (x2, y2) with a radius of r2.
For example:

var lineargradient = ctx.createLinearGradient(0, 0, 150, 150);
var radialgradient = ctx.createRadialGradient(75, 75, 0, 75, 75, 100);

Once we've created a CanvasGradient object we can assign colors to it by using the addColorStop() method.

gradient.addColorStop(position, color)
Creates a new color stop on the gradient object. The position is a number between 0.0 and 1.0 and defines the relative position of the color in the gradient, and the color argument must be a string representing a CSS , indicating the color the gradient should reach at that offset into the transition.

# Styling text


font = value
The current text style being used when drawing text. This string uses the same syntax as the CSS font property. The default font is 10px sans-serif.
textAlign = value
Text alignment setting. Possible values: start, end, left, right or center. The default value is start.
textBaseline = value
Baseline alignment setting. Possible values: top, hanging, middle, alphabetic, ideographic, bottom. The default value is alphabetic.
direction = value
irectionality. Possible values: ltr, rtl, inherit. The default value is inherit.
 (Links to an external site.)Advanced text measurements
In the case you need to obtain more details about the text, the following method allows you to measure it.

measureText()
Returns a TextMetrics object containing the width, in pixels, that the specified text will be when drawn in the current text style.