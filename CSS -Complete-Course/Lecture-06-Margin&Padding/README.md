## margin
CSS Margins
Margins are used to create space around elements, outside of any defined borders.

This element has a margin of 70px.
CSS Margins
The CSS margin properties are used to create space around elements, outside of any defined borders.

With CSS, you have full control over the margins. There are properties for setting the margin for each side of an element (top, right, bottom, and left).

Margin - Individual Sides
CSS has properties for specifying the margin for each side of an element:

margin-top
margin-right
margin-bottom
margin-left
All the margin properties can have the following values:

auto - the browser calculates the margin
length - specifies a margin in px, pt, cm, etc.
% - specifies a margin in % of the width of the containing element
inherit - specifies that the margin should be inherited from the parent element
Tip: Negative values are allowed.

Example
Set different margins for all four sides of a <p> element:

p {
  margin-top: 100px;
  margin-bottom: 100px;
  margin-right: 150px;
  margin-left: 80px;
}
Margin - Shorthand Property
To shorten the code, it is possible to specify all the margin properties in one property.

The margin property is a shorthand property for the following individual margin properties:

margin-top
margin-right
margin-bottom
margin-left
So, here is how it works:

If the margin property has four values:

margin: 25px 50px 75px 100px;
top margin is 25px
right margin is 50px
bottom margin is 75px
left margin is 100px
Example
Use the margin shorthand property with four values:

p {
  margin: 25px 50px 75px 100px;
}
If the margin property has three values:

margin: 25px 50px 75px;
top margin is 25px
right and left margins are 50px
bottom margin is 75px
Example
Use the margin shorthand property with three values: 

p {
  margin: 25px 50px 75px;
}
If the margin property has two values:

margin: 25px 50px;
top and bottom margins are 25px
right and left margins are 50px
Example
Use the margin shorthand property with two values: 

p {
  margin: 25px 50px;
}
If the margin property has one value:

margin: 25px;
all four margins are 25px
Example
Use the margin shorthand property with one value: 

p {
  margin: 25px;
}
The auto Value
You can set the margin property to auto to horizontally center the element within its container.

The element will then take up the specified width, and the remaining space will be split equally between the left and right margins.

Example
Use margin: auto:

div {
  width: 300px;
  margin: auto;
  border: 1px solid red;
}
The inherit Value
This example lets the left margin of the <p class="ex1"> element be inherited from the parent element (<div>):

Example
Use of the inherit value:

div {
  border: 1px solid red;
  margin-left: 100px;
}

p.ex1 {
  margin-left: inherit;
}



CSS Margin Collapse
Sometimes two margins collapse into a single margin.

Margin Collapse
Top and bottom margins of elements are sometimes collapsed into a single margin that is equal to the largest of the two margins.

This does not happen on left and right margins! Only top and bottom margins!

Look at the following example:

Example
Demonstration of margin collapse:

h1 {
  margin: 0 0 50px 0;
}

h2 {
  margin: 20px 0 0 0;
}
In the example above, the <h1> element has a bottom margin of 50px and the <h2> element has a top margin set to 20px.

Common sense would seem to suggest that the vertical margin between the <h1> and the <h2> would be a total of 70px (50px + 20px). But due to margin collapse, the actual margin ends up being 50px.




## padding


CSS Padding
Padding is used to create space around an element's content, inside of any defined borders.

This element has a padding of 70px.

CSS Padding
The CSS padding properties are used to generate space around an element's content, inside of any defined borders.

With CSS, you have full control over the padding. There are properties for setting the padding for each side of an element (top, right, bottom, and left).

Padding - Individual Sides
CSS has properties for specifying the padding for each side of an element:

padding-top
padding-right
padding-bottom
padding-left
All the padding properties can have the following values:

length - specifies a padding in px, pt, cm, etc.
% - specifies a padding in % of the width of the containing element
inherit - specifies that the padding should be inherited from the parent element
Note: Negative values are not allowed.

Example
Set different padding for all four sides of a <div> element:  

div {
  padding-top: 50px;
  padding-right: 30px;
  padding-bottom: 50px;
  padding-left: 80px;
}
Padding - Shorthand Property
To shorten the code, it is possible to specify all the padding properties in one property.

The padding property is a shorthand property for the following individual padding properties:

padding-top
padding-right
padding-bottom
padding-left
So, here is how it works:

If the padding property has four values:

padding: 25px 50px 75px 100px;
top padding is 25px
right padding is 50px
bottom padding is 75px
left padding is 100px
Example
Use the padding shorthand property with four values:

div {
  padding: 25px 50px 75px 100px;
}
If the padding property has three values:

padding: 25px 50px 75px;
top padding is 25px
right and left paddings are 50px
bottom padding is 75px
Example
Use the padding shorthand property with three values: 

div {
  padding: 25px 50px 75px;
}
If the padding property has two values:

padding: 25px 50px;
top and bottom paddings are 25px
right and left paddings are 50px
Example
Use the padding shorthand property with two values: 

div {
  padding: 25px 50px;
}
If the padding property has one value:

padding: 25px;
all four paddings are 25px
Example
Use the padding shorthand property with one value: 

div {
  padding: 25px;
}
Padding and Element Width
The CSS width property specifies the width of the element's content area. The content area is the portion inside the padding, border, and margin of an element (the box model).

So, if an element has a specified width, the padding added to that element will be added to the total width of the element. This is often an undesirable result.

Example
Here, the <div> element is given a width of 300px. However, the actual width of the <div> element will be 350px (300px + 25px of left padding + 25px of right padding):

div {
  width: 300px;
  padding: 25px;
}
To keep the width at 300px, no matter the amount of padding, you can use the box-sizing property. This causes the element to maintain its actual width; if you increase the padding, the available content space will decrease.

Example
Use the box-sizing property to keep the width at 300px, no matter the amount of padding:

div {
  width: 300px;
  padding: 25px;
  box-sizing: border-box;
}




## height and Width


CSS Height, Width and Max-width
The CSS height and width properties are used to set the height and width of an element.

The CSS max-width property is used to set the maximum width of an element.

This element has a height of 50 pixels and a width of 100%.

CSS Setting height and width
The height and width properties are used to set the height and width of an element.

The height and width properties do not include padding, borders, or margins. It sets the height/width of the area inside the padding, border, and margin of the element.

CSS height and width Values
The height and width properties may have the following values:

auto - This is default. The browser calculates the height and width
length - Defines the height/width in px, cm, etc.
% - Defines the height/width in percent of the containing block
initial - Sets the height/width to its default value
inherit - The height/width will be inherited from its parent value
CSS height and width Examples
This element has a height of 200 pixels and a width of 50%
Example
Set the height and width of a <div> element:

div {
  height: 200px;
  width: 50%;
  background-color: powderblue;
}

This element has a height of 100 pixels and a width of 500 pixels.
Example
Set the height and width of another <div> element:

div {
  height: 100px;
  width: 500px;
  background-color: powderblue;
}

Note: Remember that the height and width properties do not include padding, borders, or margins! They set the height/width of the area inside the padding, border, and margin of the element!

Setting max-width
The max-width property is used to set the maximum width of an element.

The max-width can be specified in length values, like px, cm, etc., or in percent (%) of the containing block, or set to none (this is default. Means that there is no maximum width).

The problem with the <div> above occurs when the browser window is smaller than the width of the element (500px). The browser then adds a horizontal scrollbar to the page.

Using max-width instead, in this situation, will improve the browser's handling of small windows.

Tip: Drag the browser window to smaller than 500px wide, to see the difference between the two divs!

This element has a height of 100 pixels and a max-width of 500 pixels.
Note: If you for some reason use both the width property and the max-width property on the same element, and the value of the width property is larger than the max-width property; the max-width property will be used (and the width property will be ignored).

Example
This <div> element has a height of 100 pixels and a max-width of 500 pixels: 

div {
  max-width: 500px;
  height: 100px;
  background-color: powderblue;
}


