# ch 5 : IMAGES 
you could add image to a web page if you want to include a logo,photograph,diagram,or chart.

```
<img src= "put the path here "alt="descripition of the img" width="600" height="450"/>
``` 

Where to place image in your code : 
* before a paragraph

```
<img scr="the path" alt="description"/><p>abcdefg</p>
```

* inside the start of a paragraph

```
<p><img src="the path" alt="the alt"/>abcdefg</p>
```

* in the midele of paragraph 

```
<p>abcd<img src="path" alt="alt"/>efghi</p>
```


## tool to Edit and save images

**the most** popular tool is Adobe Photoshop.


## Figure and Figure Caption 

`<figure>`

You can have more than one
image inside the `<figure>`
element as long as they all share
the same caption.

`<figcaption>`

to allow web page authors to add
a caption to an image.

# ch 11: color 

color bring your pages to life .

## forground color 

**color** 

```
h1{
    color : red;
}
```

## background color 

```
body{
background-color : red;
}
```

# ch 12 : Text 

## typeface terminology 

* **serif**
* **sans-serif**

* **monospace**


## specifing typefaces 

***font-family***

```
body {
    font-family : Arial, verdana,sans-serif;
}
```

## size of type

***font-size***

```
body{
    font-size:12px;
}
```

## bold 
***font-weight***

```
body{
    font-weight:bold;
}
```

## italic 

```
body{
    font-style:italic;
}
```

## uppercase and lowercase

**text-transform**

```
h3{
text-transform : uppercase;
}
```

## underline and strike

***text-decoration***

* none
* underline
* overline
* line-through
* blink

```
.c{
    text-decoration : underline;
}
```

## letter and word spacing 

**letter-spacing** 

**word-spacing**

```
h1{
    letter-spacing:0.2 em;
}
h2{
    word-spacing:1em;
}
```

## alignment
**text-align**

```
h1{
    text-align:right;
}
```

## vertical alignment 

```
#m
{
vertical-align:baseline;
}
```

## drop shadow

**text-shadow**

```
p.one{
    text-shadow:1px 1px 3px #cccccc
}
```

## first letter and first line

```
p:first-letter{
font-size:200%;
}
```

## styling links 

```
a:link{
    color:deeppink;
    text-decoration:none;
}
```

## JPEG vs PNG vs GIF

Use JPEG format for all images that contain a natural scene or photograph where variation in colour and intensity is smooth. Use PNG format for any image that needs transparency or for images with text & objects with sharp contrast edges like logos. Use GIF format for images that contain animations.

## Compression
Almost all forms of data that we see on the internet are compressed to reduce the size of data and ensure faster transmission. Choosing the correct format and compression is a major factor that determines image size.


* **JPEG** is a lossy compression specification that takes advantage of human perception. It can achieve compression ratios of 1:10 without any perceivable difference in quality.PEG images are best suited for photographs and paintings of natural scenes where the variations in colour and intensity are smooth.


* **PNG** is a lossless image format No data is lost during compression and no compression artefacts are introduced in the image. For this reason, a PNG image would retain higher quality than an image than JPEG and would look a lot sharper, it would also occupy more space on the disk. This makes it unsuitable for storing or transferring high-resolution digital photographs but a great choice for images with text, logos and shapes with sharp edges.


* **GIF** is also a lossless image format that uses LZW compression algorithm. It was favoured over PNG for simple graphics in websites in its early days because the support of PNG was still growing. Given that PNG is now supported across all major devices and that PNG compression is about 5–25% better than GIF compression, GIF images are now mainly used only if the image contains animations.

## Transparency

transparency indicates something that is completely invisible. Logos and icons often need to be placed on backgrounds with variable colours. Hence it is desirable, that the background of these logos and icons is made transparent so that a single image can be used over multiple background variations.

* **JPEG** images don’t support transparency and are hence not usable for such cases.

* **PNG** images support transparency in two ways — inserting an alpha channel that allows partial transparency or by declaring a single colour as transparent 

* **GIF** images support transparency by declaring a single colour in the colour palette as transparent

## Colours

* **JPEG** images can support around 16 million colours. This is what makes them suitable for storing images of natural scenes.

* **PNG** images mainly have two modes — PNG8 and PNG24. PNG8 can support upto 256 colours whereas PNG24 can handle upto 16 million colours like a JPEG image. 

* **GIF** images are limited to 256 colours. If index transparency is used, then one of these 256 colours is assigned as transparent and the remaining 255 are used for other colours.

## Animation

Of these 3 formats, only **GIF** supports animation.

