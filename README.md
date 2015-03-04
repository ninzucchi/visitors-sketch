# Sketch 101 Cambridge Class

## *Lovingly taught by one Nicholas W. Inzucchi*

Prerequisite software installs:

[Sketch 3.2.2 Demo](http://bohemiancoding.com/sketch/)

Sketch emerged to fill what was, in retrospect, a tremendously obvious need: Digital designers need a digital tool to design digital tools. Sketch entirely focused on UI design. The competitors it disrupts, namely Photoshop and Illustrator, were burdened by years of cruft; hundreds of features and settings for photos and print that distract from our core purpose.

Because if its tremendous focus, Sketch has quickly sparked a revolution in digital design. For starters: 

- **Vector-Based** : Vector assets make exporting to multiple devices is a breeze. 
- **Pixel Snap/Zoom** : Be confident designs on desktop will look exactly the same on a device.
- **Mirror** : A built-in iPhone previewing makes for a hyper-efficient tweaking.
- **Text Rendering** : 100% accurate rendering across retina screens and sub-pixel aliased devices.
- **Rapid Exports** : No more bullshit file renaming. Set names once and use a single shortcut to render out.

Ready? Let’s begin.

The world can never have enough sadistic dating apps. In this workshop, that’ll be our goal.

# Basic Interface

## Toolbar

![toolbar](https://raw.github.com/ninzucchi/visitors-cambridge/master/img/toolbar.png)

The toolbar contains helpful icons represening basic operations. This area is mostly a crutch for beginner usability. As you begin master keyboard shortcuts its utility will steadily decrease. I really use mine only for boolean operations and mirroring.

## Layers List
The Layers list shows, as you might guess, a list of layers on the current page. Remember how much memory Illustrator or Photoshop hog? Pages are Sketch’s attempt at a fix. Use them to split huge files into multiple pieces and keep performance consistently high.

## Inspector
If you’ve used keynote, you’re likely familiar with the inspector. It shows the properties and attributes of the currently selected object. *Note to Adobe Converts : Sketch has no concept of a Select tool so you can stop pressing ‘v’ all the time. Instead, use ‘esc’ to return to a normal cursor.*

# Art boards

Fire up Sketch and the first thing you’ll see is a blank, infinite canvas. You can work here just fine, but pretty quickly  you’ll see a need to keep things organized. To do that, you’ll need an art board. Art boards are the skeleton of your app, and you’ll need one per screen.

To create an art board press (A). The inspector updates to show several common sizing options. Rejoice, no more Googling screen resolutions! Let’s select **iPhone Portrait**.

Nice. Art boards can be selected in the Layers List, or by clicking their name on the canvas. Go ahead and select the current art board.

# Layers

Everything in Sketch is a layer. These are its basic building blocks. Every shape, object, and piece of type is treated identically: as a Layer.

## Basic Shapes

To add a new layer, click the Insert icon in the toolbar. Our app needs a little header, so let’s add a Rectangle. Drag anywhere on the art board to create your Rectangle, then check out the inspector.

### Editing Properties

Every layer in Sketch has the same set of basic properties: Position, Size and Transform. Type directly in these boxes to set your header’s position to (0,0) and its size to a slim (640,15).

One of Sketch’s most useful features is the ability to use algebra in inspector fields. In the upcoming beta, you can even use percentages. Use this feature to keep get your anal-retentive rocks off.

### Color
Every layer also has appearance properties. These include opacity, blend mode, fills, borders, shadows, and blur. Let’s begin with color. Click the color swatch in your header’s ‘Fills’ field. 

Sketch’s color selector is pretty great. Consistent with the digital-first mindset, it accepts Hex codes and uses HSLA by default. Sketch automatically detects the colors present in your current design and adds them to the first row of swatches. If that’s not enough, you can always add the current color to the second row of swatches by pressing ‘+’.

Select something nice and bright, then deselect the Rectangle by clicking anywhere else within the canvas.

Similar to colors, the typefaces that are used in your current design will be automatically detected.

## Guides
Our interface needs a nice background, so let’s create another rectangle. This time, use the (R) shortcut key to equip the Rectangle tool. We’ll use guides to draw the perfect shape. Begin drawing near the dartboard’s top-left corner, drag to the bottom-right, and release. As you drag, your cursor will snap to nearby edges. This feature makes it quite efficient to draw by hand.

## Layer Manipulation
Our new rectangle is on top of the layer stack, and that’s no good. In the Layer List, drag its name to the bottom of the list. 

While we’re here, let’s do some renaming. Double click on the art board name, ‘Portrait,’ and rename it to ‘Home.’ Before you confirm, try pressing Tab to automatically jump to the next title. Rename your remaining layers this way.

### Advanced Color
That background would look great with a subtle dark gradient. Click its fill swatch and select the Linear Gradient tab/icon at the top of the popup. I won’t attempt to explain how to build a gradient in words, but take a stab at something dark & sexy.

FYI there are also fill tabs for Radial Gradients, Angular Gradients, Patterns and Noise fills.

## Paths
Let’s make a quick ‘close’ icon to begin working with Paths. Press ‘L’ to enter the line tool. Hold shift and draw a line at 45 degrees. Change the line’s stroke color to white, and give it rounded end caps. Now Duplicate that shape and press ‘flip horizontal’. This produces an X.

Strokes can be converted to shapes with the ‘Vectorize Stroke’ command. Let’s use this now to make a proper icon. Vectorize both lines to convert them to real shapes.

## Boolean Operations
After converting both lines, we’ll want to combine them into a single shape. Sketch’s Boolean operations provide a perfect utility for this purpose. Select both lines then Layer > Combine > Union. This merges both shapes into a single form. In the Layer List, the source shapes appear nested together as if in a folder. Rest assured, they are combined. This merely allows us to edit the source components directly if necessary.   

# Images

## Principles
Images drop onto the canvas just like shapes. They also have all the same properties, such as fill and stroke. Images are embedded into the file; there is currently no way to live link to external files. If you need to update an image asset, Layer > Image > Replace… is a helpful command to know.

Any selection can be flattened into an image. If heavily stacked, dynamic blurred backgrounds or deeply layered interface can cause a loss of performance, especially if present on many art boards. Pages can help, and flattening layers is another powerful weapon.

## Masks
In Sketch, any layer can serve as a mask for other layers/folders at the same level of hierarchy. To turn a layer into a mask, right click its title in the Layers List and select ‘Use as Mask.’ All layers that are both above the mask and within its  same container will now be clipped by this shape. Masks can’t apply outside their current folder, so use folders wisely to keep things in check. Alpha Masks are also available through Layer > Mask Mode > Alpha Mask.

# Reusability

Is the shit!

## Shared Styles

Shared styles allow you to effortlessly share a single set of physical attributes across many shapes. A Shared Style saves information in all of the inspector fields below the ’Shared Style’ dropdown, namely Fill, Border, Shadow, Inner Shadow, Blur, and Color Adjust.

Let’s use Shared Styles to unite our iconography. First select the ‘X’ icon. In the inspector, open the Shared Style dropdown and choose ‘Create New Shared Style.’ Give it a name and press Enter. Now, with the Heart icon selected, choose the Shared Style you created. Done! To make sure things worked as planned, change the Heart’s fill to pink. The ‘X’ should update immediately.   

## Text Styles

Text Styles work just like Shared Styles. In addition to the physical attributes of Shared Styles, Text styles also store typographic information like Font and Paragraph settings.

Even if you’re not planning to reuse a given style, it can be helpful to keep them cataloged. Fewer is better, after all. Let’s give Text Styles to all of the type we’ve employed so far.

## Symbols

The team had to rethink about how Symbols could be designed in the context of Sketch. As I was using it during the beta, I was amazed; it works effectively across Artboards. You don’t need to go back and edit re-used headers, footers and buttons anymore. They just update on the fly and at a fantastic performance.

# Exporting
In order to make any art board, layer, or group exportable simply select it and click ‘Make Exportable’ in the inspector. This reveals a button to export that particular item, and also makes the item appear in the popup resulting from File > Export… Exported Layers are named with their layer names within Sketch, so be sure to keep that shit tight! 

## Drag n Drop
Sketch allows for simply dragging art boards outside the app window to export. Multiple Artboards work the same. Select multiple to see their previews render in the inspector, ready to be dragged out for a quick export.

## Slices
Sketch also supports good old fashioned slices. A slice is an invisible rectangle that, when exported, renders all pixels contained within. Slices always appear in the File > Export… menu.

## Batching
The most powerful and useful way to export layers is using File > Export… This popup contains line items for every dartboard, slice, and/or layer marked as ‘Exportable.’ Exported layers automatically overwrite older versions, making this an incredibly painless flow. Memorize ‘Cmd + Shift + E’ and reap untold benefits. 

Any exportable object can be programmed to export at multiple resolutions. Just put a multiplier (e.g. 1x, 2x, 3x) pixel size (e.g. 700h, 300w) or pixel density (e.g. 150dpi, 300dpi) in the ‘Size’ input of the selected object.

## CSS Styles
This feature is especially useful for getting the colors, border-radius, fonts and gradient properties. As a coder, I always suggest that you code manually in order to give yourself the flexibility to change things and make them adaptable to different browsers / devices.

# Mirroring

Sketch can mirror natively to any iOS device, it’s dope! 

# Pro Tips

## Presentation Mode

A fantastic way to present your UI to your co-workers without the noises. Just press Command + .

## iCloud Versions

Sketch has Autosave enabled. It keeps the versioning of your files, so you no longer run into the problem of having to save files manually or risk losing edits. To restore an old version, go to File / Revert To / Browse All Versions.

## Layout Grids

If you love layout grids such as the 960grid, then you’re in luck. Sketch has a fantastic Grid feature. You can create virtually any grid you’d like. This is particularly helpful for the Web.

## Opacity Keys

When you select a Layer or a Group and press the 1 key, it’ll set it to 10% opacity.
