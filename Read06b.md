# How to make your web pages more attractive?

Controlling the design of the them using CSS .

CSS allows you to create rules that specify how the content of
an element should appear.

### Understanding CSS :thinking inside the box 

The key to understanding how CSS works is to
imagine that there is an invisible box around every HTML element.
There is a difference between block level and inline elements and how browser display them .

* Block level elements look like they start on new line .

Examples include the `<h1>`- `<h6>` and `<div>` elements .

* Inline elements flow within the text and do not start on a new line .
Examples include `<b>` , `<i>`,`<img>`,`<em>`,`<span>`.

## Example styles : 

* Boxes : 

width and height borders (color,width,and style)
Background color and images position in the browser window 

* Text : 

Size ,color ,italics,bold,uppercase,lowercase

* Specific :

there are also specific ways in which you can style certain elements such as lists,tables and forms

## Css associates style rules with html elements :
CSS works by associating rules with HTML elements. These rules govern how the content of specified elements should be displayed. 

A CSS rule contains two parts: a **selector** and a **declaration**.

```
P {
Font-family : arial;
}
```
 
This rule indicates that all `<p>`elements should be shown in the
Arial typeface.

**Selectors** indicate which
element the rule applies to.
The same rule can apply to more than one element if you separate the element names with commas.

**Declarations** indicate how the elements referred to in the selector should be styled.
Declarations are split into two parts (a property and a value), and are separated by a colon.

### CSS Properties Affect How Elements Are Displayed :

CSS declarations sit inside curly brackets and each is made up of two parts: a **property** and a **value**, separated by a colon. 

You can specify several properties in one declaration, each separated by a semi-colon.

```
h1, h2, h3 {
font-family: Arial;
color: yellow;}
```

This rule indicates that all `<h1>`,`<h2>` and `<h3>` elements should be shown in the Arial typeface, in a yellow color.

* Properties indicate the aspects of the element you want to change. For example, color, font, width, height and border.

* Values specify the settings you want to use for the chosen properties. For example, if you want to specify a color property
then the value is the color you want the text in these elements
to be.

Example 

```
DOCTYPE html>
<html>
<head>
<title>Introducing CSS</title>
<link href="css/example.css" type="text/css"
rel="stylesheet" />
</head>
<body>
<h1>From Garden to Plate</h1>
<p>A <i>potager</i> is a French term for an
ornamental vegetable or kitchen garden ... </p>
<h2>What to Plant</h2>
<p>Plants are chosen as much for their functionality
as for their color and form ... </p>
</body>
</html>

body {
font-family: Arial, Verdana, sans-serif;}
h1, h2 {
color: #ee3e80;}
p {
color: #665544;}
```

`<link>` external-css.html  
The `<link>` element can be used in an HTML document to tell the
browser where to find the CSS file used to style the page. It is an empty element (meaning it does not need a closing tag), and it
lives inside the `<head>` element.

It should use three attributes:
* href
This specifies the path to the CSS file (which is often placed in
a folder called css or styles).

* type
This attribute specifies the type of document being linked to. The
value should be text/css.

* rel
This specifies the relationship between the HTML page and
the file it is linked to. The value should be stylesheet when
linking to a CSS file.

Using internal css :

```
<!DOCTYPE html>
<html>
<head>
<title>Using Internal CSS</title>
<style type="text/css">
body {
font-family: arial;
background-color: rgb(185,179,175);}
h1 {
color: rgb(255,255,255);}
</style>
</head>
<body>
<h1>Potatoes</h1>
<p>There are dozens of different potato
varieties. They are usually described as
early, second early and maincrop.</p>
</body>
</html>
```

`<style>`

You can also include CSS rules within an HTML page by placing
them inside a `<style>` element, which usually sits inside the
`<head>` element of the page.

The `<style>` element should use the type attribute to indicate
that the styles are specified in CSS. The value should be text/
css.

***

* Universal selector `*{}` target all elements on the page 
* Type selector `h1,h2,h3 {} ` targets the `<h1>`,`<h2>`,`<h3>`
* Class selector `.note{}`
* Id selector `#introduction{}`
* Child selector `li>a{}`
* Descendant selector `p a {}`

# ch 11 

Color can really bring your pages to life.

* Foreground Color

```
/* color name */
h1 {
color: DarkCyan;}
/* hex code */
h2 {
color: #ee3e80;}
/* rgb value */
p {
color: rgb(100,100,90);}
```

* Background color 

```
body {
background-color: rgb(200,200,200);}
h1 {
background-color: DarkCyan;}
h2 {
background-color: #ee3e80;}
p {
background-color: white;}
```
*** 

1. RGB Values
Values for red, green, and blue
are expressed as numbers between 0 and 255 

3. Hex Codes
Hex values represent values
for red, green, and blue in
hexadecimal code.

6. Color Names
Colors are represented by
predefined names. However,
they are very limited in number.