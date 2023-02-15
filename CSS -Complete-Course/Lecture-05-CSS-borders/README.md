# Lecture 4

## Borders
CSS border properties allow you to specify the style, width, and color of an element's border.

I have borders on all sides.


I have a red bottom border.


I have rounded borders.


I have a blue left border.

CSS Border Style
The border-style property specifies what kind of border to display.

The following values are allowed:

dotted - Defines a dotted border
dashed - Defines a dashed border
solid - Defines a solid border
double - Defines a double border
groove - Defines a 3D grooved border. The effect depends on the border-color value
ridge - Defines a 3D ridged border. The effect depends on the border-color value
inset - Defines a 3D inset border. The effect depends on the border-color value
outset - Defines a 3D outset border. The effect depends on the border-color value
none - Defines no border
hidden - Defines a hidden border
The border-style property can have from one to four values (for the top border, right border, bottom border, and the left border).

Example
Demonstration of the different border styles:

p.dotted {border-style: dotted;}
p.dashed {border-style: dashed;}
p.solid {border-style: solid;}
p.double {border-style: double;}
p.groove {border-style: groove;}
p.ridge {border-style: ridge;}
p.inset {border-style: inset;}
p.outset {border-style: outset;}
p.none {border-style: none;}
p.hidden {border-style: hidden;}
p.mix {border-style: dotted dashed solid double;}
Result:

A dotted border.

A dashed border.

A solid border.

A double border.

A groove border. The effect depends on the border-color value.

A ridge border. The effect depends on the border-color value.

An inset border. The effect depends on the border-color value.

An outset border. The effect depends on the border-color value.

No border.

A hidden border.

A mixed border.

Note: None of the OTHER CSS border properties (which you will learn more about in the next chapters) will have ANY effect unless the border-style property is set!
## Border Sides
CSS Border Width
The border-width property specifies the width of the four borders.

The width can be set as a specific size (in px, pt, cm, em, etc) or by using one of the three pre-defined values: thin, medium, or thick:

Example
Demonstration of the different border widths:

p.one {
  border-style: solid;
  border-width: 5px;
}

p.two {
  border-style: solid;
  border-width: medium;
}

p.three {
  border-style: dotted;
  border-width: 2px;
}

p.four {
  border-style: dotted;
  border-width: thick;
}
Result:

5px border-width
medium border-width
2px border-width
thick border-width
Specific Side Widths
The border-width property can have from one to four values (for the top border, right border, bottom border, and the left border):

Example
p.one {
  border-style: solid;
  border-width: 5px 20px; /* 5px top and bottom, 20px on the sides */
}

p.two {
  border-style: solid;
  border-width: 20px 5px; /* 20px top and bottom, 5px on the sides */
}

p.three {
  border-style: solid;
  border-width: 25px 10px 4px 35px; /* 25px top, 10px right, 4px bottom and 35px left */
}
## Border width
CSS Border Color
The border-color property is used to set the color of the four borders.

The color can be set by:

name - specify a color name, like "red"
HEX - specify a HEX value, like "#ff0000"
RGB - specify a RGB value, like "rgb(255,0,0)"
HSL - specify a HSL value, like "hsl(0, 100%, 50%)"
transparent
Note: If border-color is not set, it inherits the color of the element.

Example
Demonstration of the different border colors:

p.one {
  border-style: solid;
  border-color: red;
}

p.two {
  border-style: solid;
  border-color: green;
}

p.three {
  border-style: dotted;
  border-color: blue;
}
Result:

Red border
Green border
Blue border
Specific Side Colors
The border-color property can have from one to four values (for the top border, right border, bottom border, and the left border). 

Example
p.one {
  border-style: solid;
  border-color: red green blue yellow; /* red top, green right, blue bottom and yellow left */
}
HEX Values
The color of the border can also be specified using a hexadecimal value (HEX):

Example
p.one {
  border-style: solid;
  border-color: #ff0000; /* red */
}
RGB Values
Or by using RGB values:

Example
p.one {
  border-style: solid;
  border-color: rgb(255, 0, 0); /* red */
}
HSL Values
You can also use HSL values:

Example
p.one {
  border-style: solid;
  border-color: hsl(0, 100%, 50%); /* red */
}
You can learn more about HEX, RGB and HSL values in our CSS Colors chapters.
## Border Color

## Border Shorthand
CSS Border - Shorthand Property
Like you saw in the previous page, there are many properties to consider when dealing with borders.

To shorten the code, it is also possible to specify all the individual border properties in one property.

The border property is a shorthand property for the following individual border properties:

border-width
border-style (required)
border-color
Example
p {
  border: 5px solid red;
}
Result:

Some text

You can also specify all the individual border properties for just one side:

Left Border
p {
  border-left: 6px solid red;
}
Result:

Some text

Bottom Border
p {
  border-bottom: 6px solid red;
}
Result:

Some text
## Rounder Borders
CSS Rounded Borders
The border-radius property is used to add rounded borders to an element:

Normal border

Round border

Rounder border

Roundest border

Example
p {
  border: 2px solid red;
  border-radius: 5px;
}
## border sides

CSS Border - Individual Sides
From the examples on the previous pages, you have seen that it is possible to specify a different border for each side.

In CSS, there are also properties for specifying each of the borders (top, right, bottom, and left):

Example
p {
  border-top-style: dotted;
  border-right-style: solid;
  border-bottom-style: dotted;
  border-left-style: solid;
}
Result:

Different Border Styles
The example above gives the same result as this:

Example
p {
  border-style: dotted solid;
}
So, here is how it works:

If the border-style property has four values:

border-style: dotted solid double dashed;
top border is dotted
right border is solid
bottom border is double
left border is dashed
If the border-style property has three values:

border-style: dotted solid double;
top border is dotted
right and left borders are solid
bottom border is double
If the border-style property has two values:

border-style: dotted solid;
top and bottom borders are dotted
right and left borders are solid
If the border-style property has one value:

border-style: dotted;
all four borders are dotted
Example
/* Four values */
p {
  border-style: dotted solid double dashed;
}

/* Three values */
p {
  border-style: dotted solid double;
}

/* Two values */
p {
  border-style: dotted solid;
}

/* One value */
p {
  border-style: dotted;
}
The border-style property is used in the example above. However, it also works with border-width and border-color.