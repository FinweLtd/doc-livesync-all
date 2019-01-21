# Understanding Resolution in 360°

![Cover](img/StockSnap_UDUTMK0974_edited.jpg)

## Definition

First, let us define what we mean by *image resolution*.

> Image resolution is the detail an image holds ... Higher resolution means more image detail. ([1])

The concept of image resolution applies to *raster digital images* ([2]), such as JPG, PNG and BMP
images. It is important to differentiate images created with *vector graphics* ([3]), such as SVG
images, as they are defined mathematically and image resolution for such images becomes meaningful
only when the image is saved in a different format (rasterized to JPG, for instance). 

Digital cameras produce raster images. Therefore, 360-degree images are raster images just like 
any other photograph or video frame is. Sometimes 360-degree images are not captured with a real
camera, but *rendered* from a mathematical model (such as a CAD model of a building) using a virtual
camera. The concept of resolution applies to the rasterized output file.

To be specific, in this article we will discuss *pixel resolution* ie. the pixel count in the 
image, not *spatial resolution* (how closely lines can be resolved in an image - for example from
a printed photograph) or *spectral resolution* (the ability to resolve spectral features and bands
- for example colors). From now on, when we use the word *resolution* we mean pixel resolution.

![Resolution Illustration](https://upload.wikimedia.org/wikipedia/commons/f/f2/Resolution_illustration.png)

*Pixel resolution illustration by Wikipedia ([1])*

## Describing Resolution

There are several methods to describe image resolution. In this article, we will use many of them:

> ... the convention is to describe the pixel resolution with the set of two positive integer 
> numbers, where the first number is the number of pixel columns (width) and the second is the 
> number of pixel rows (height), for example as 7680 × 6876. Another popular convention is to 
> cite resolution as the total number of pixels in the image, typically given as number of 
> megapixels, which can be calculated by multiplying pixel columns by pixel rows and dividing 
> by one million. Other conventions include describing pixels per length unit or pixels per area 
> unit, such as pixels per inch or per square inch. ([1])

As an example, the image below is 1024 pixels wide and 1024 pixels tall and we can express its
resolution as 1024 x 1024 pixels (width x height). We can also calculate the total number of pixels
the image contains simply by multiplying width and height:

```
1024 px x 1024 px = 1048576 px
```

By dividing this value by one million, we get the resolution in megapixels:

```
1048576 px / 1000000 = 1.048576 MPx ~ 1 MPx
```

In other words, this image has 1 megapixel resolution, and it looks pretty sharp on screen.

![Cube Front](img_resolution/Orion360_test_image_front.png)

We cannot say much about its number of pixels *per length unit* or *per area unit*, because its 
size will be *scaled* to match with the width of this text column, and the size of this text 
column in millimeters (or inches) depends on the display device and window size where the content
is rendered to. For example, on a tablet screen the width could be 163 mm, hence we could say
that its resolution is about 6 pixels per millimeter - but only in this particular case!

```
1024 px / 163 mm = ~6.28 px/mm
```

For example, if you are reading this from a computer screen, try resizing the width
of your browser window: you should see that the image above will be automatically resized. The
resolution of the original image file that your browser has downloaded remains the same,
but what you see on screen is actually a *copy* of the original image, which your browser has
created and scaled to match with this column's width. That copy probably has a different 
resolution than the original file does.

It is important to understand the difference between the resolution of an image in a file
and on screen. Consider the image above: what if its (file) resolution would be reduced to
10 x 10 pixels? Certainly it would become a blurry mess. On screen, it would be still scaled
to match with the width of this column. Obviously, your computer must use much more than 10 x 10 
pixels to draw the image on screen since the display pixel are really small - but it cannot 
magically recreate the detail that was lost when we scaled down the original image. Hence,
all it can do is to copy the exact same pixel values side by side to create a larger image. 
The resulting image would have lots of pixels, but its *spatial resolution* would be really low!

So far we haven't said anything about resolution in 360-degree images. Let's first create one:
We will use the image above as a single cube face and make 5 more copies of it to produce the
six faces that are required for a cube. Then we can put a virtual camera inside the cube, to
its center point, and render a spherical 360-degree image. In order to save that 3D image into
a PNG file, we must choose *a projection* that can be used for projecting a sphere into a planar
surface, just like we project a map of our dear planet Earth to a piece of paper (that is topic
of its own for another article). For simplicity, we will use equirectangular projection.

![Cube Equi](img_resolution/Orion360_test_image_equi.jpg)












[1]: https://en.wikipedia.org/wiki/Image_resolution
[2]: https://en.wikipedia.org/wiki/Raster_graphics
[3]: https://en.wikipedia.org/wiki/Vector_graphics

