# NeoTrellis Keycaps
These are 3D-printable keycaps for the [Adafruit Silicone Elastomer Button Keypads](https://www.adafruit.com/product/1611).

## Purpose:
The 'Silicone Elastomer' button keypad material resists being written on or having anything stuck to it for labeling.
So I've designed 3D-printable keycaps to fit snugly over the silicone buttons.
They push down over the buttons and stay in place rather well.
Printed in black with transparent icons, they work well as functional lighted keycaps. Or go wild with the colors!

## Image of Example lamp keycap:
![Example Lamp Keycap](Trellis%20Keycap%20Lamp.png)

## Image of NeoTrellis keypad with custom keycaps:
![Image of NeoTrellis keypad with custom keycaps](NeoTrellis%20Keypad.jpg)

## Caution:
While the keycaps stay in place with normal use, they can be removed easily with the fingers.
So you should keep these out of the reach of small children like you would with any other small objects.

## Concept:
A few directly usable keycap designs are provided as examples in OBJ format. The original blank keycap template
was created in [Fusion 360](https://www.autodesk.com/products/fusion-360/personal), so the customization process
happens there as well. I've used icons from those available at 
[Material Design Icons](https://pictogrammers.com/library/mdi/) which are used by Home Assistant, so my
keypad icons can match those used in my HA dashboards.
You can use any format loadable into Fusion as a 2D sketch or draw your own, of course.
You'll want to use simple icons with no small details due to the size limitations.

## Customization:
* Load the "Trellis Keycap.f3d" file int Fusion 360
* At this point you should save the design AS another name for this new keycap to preserve the original for future use
* Insert your SVG icon file as a sketch
  * INSERT > Insert SVG
  * Insert from my computer...
  * Select the downloaded SVG icon
  * Select the bottom face of the keycap top from the inside
  * Position the icon by dragging the square box with the mouse
  * Size the icon by dragging the white arc with the mouse
  * You can use the full space of the inner face of the top
    * We're operating from the inside to better visualize those sizing limits
    * The bigger the icon, the better for most purposes
  * You may need to flip the icon horizontally as we're coming from the inside
  * OK to finish SVG insertion
  * I've found some icons to not be properly closed or complete
    * You may want to continue editing the sketch to fix this or modify the icon
  * Finish Sketch
* Cut the outline of the icon through the top face of the keycap
  * Click inside the outline of the icon in the sketch
    * This may require using ctrl+click to select multiple parts
  * Press 'E' to extrude the outline(s)
  * Enter a distance of -0.5 to cut into the face
    * This is the thickness of the top
    * If you modified that thickness, you'll need to specify that value here
    * Or you can spcify 'All' as the Extent Type
  * Specify a 'Cut' Operation
  * OK
* Fill the cut icon space with a new body
  * Make the icon sketch visible again
    * Using the eye icon in the object browser tree
  * Reselect the icon outline(s)
  * Press 'E' to extrude again
  * Specify the same distance as before
  * Select 'New Body' as the operation
  * OK
* Set a new material appearance for the icon parts for 3D printing (optional)
  * I like to visualize a clear icon by changing its material to glass
  * Press 'A' for the APPEARANCE dialog
    * You should see some preloaded materials 'In This Design'
    * The black was used on the keycap's body
  * Click and apply the glass material to the icons part(s)
  * Close
* Save the design
* Create on OBJ file for 3D printing
  * Right-click the design name at the very top of the component browser
  * Save As Mesh
    * I use the OBJ Format since the accompanying MTL file retains information about the materials used 
    * OK
  * Change the Name if you like
  * Check 'Save to my computer' and select a new path or name if you like
  * Save
* 3D printing
  * It certainly helps to have a printer that supports at least two filaments for a print
  * I use Bambu Studio and the Bambu X1 Carbon printer with AMS (Automatic Material System) to print with multiple filaments
    * That lets me easily map from the OBJ file's materials to the filaments in the AMS
    * I choose black and transparent filaments
    * You can certainly use whatever filaments you like
      * Flipping the black and transparent filamants is also a nice look
      * Even using white or other colors instead of transparent can pass a nice amount of light through
  * This takes less about 15 minutes to produce a nice print
  * Slide the new keycap onto your Trellis button and move on to the next one!
