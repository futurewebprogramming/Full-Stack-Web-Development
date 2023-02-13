# Lecture -12

## Master HTML Forms in One Video


HTML form is used to collect user input. user input is most often sent to a server for processing.

### `<form>` Element

`<form>` element is used to create an HTML form for user input

`<form> `element is a container for all different types of input elements, such as: text fields, checkboxes, radio buttons, submit buttons, etc.

```html
<form>
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname">
</form>
```

### Form Elements

### `<input> `Element

`<input>` element is the most used form element.

`<input>` element can be displayed in many ways, depending on the type attribute.


Type    | Description
------- | -----------
`<input type="text">` |	Displays single-line text
`<input type="radio">` |	Displays radio button (for selecting one of many choices)
`<input type="checkbox">` |	Displays  checkbox (for selecting zero or more of many choices)
`<input type="submit">`	| Displays submit button (for submitting form)
`<input type="button">` |	Displays clickable button

#### Text Fields

```html
<label for="fname">First name:</label>
<input type="text" id="fname" name="fname">
```
<label for="fname">First name:</label>
<input type="text" id="fname" name="fname">

### `<label>` Element

`<label>` element defines label for form elements.

`<label>` element also help users who have difficulty clicking on very small regions (such as radio buttons or checkboxes) - because when user clicks text within the `<label> `element, it toggles the radio button/checkbox.

` <label> `tag should be equal to the `id` attribute of the `<input>` element to _**bind them**_ together.

#### Input Type Password
to get password from user , 
>characters in a password field are masked (shown as asterisks or circles)

```html
<form>
  <label for="username">Username:</label><br>
  <input type="text" id="username" name="username"><br>
  <label for="pwd">Password:</label><br>
  <input type="password" id="pwd" name="pwd">
</form>
```

### Radio Buttons
`<input type="radio">` with Radio buttons user can select ONE option from given options.

```html
<p>Choose your favorite language:</p>

<form>
  <input type="radio" id="html" name="fav_language" value="HTML">
  <label for="html">HTML</label><br>
  <input type="radio" id="css" name="fav_language" value="CSS">
  <label for="css">CSS</label><br>
  <input type="radio" id="javascript" name="fav_language" value="JavaScript">
  <label for="javascript">JavaScript</label>
</form>
```

### Checkboxes
`<input type="checkbox">` with Checkboxes user can _*select*_ _***One or more***_ options of a limited number of choices.

```html
<form>
  <input type="checkbox" id="vehicle1" name="vehicle1" value="Bike">
  <label for="vehicle1"> I have a bike</label><br>
  <input type="checkbox" id="vehicle2" name="vehicle2" value="Car">
  <label for="vehicle2"> I have a car</label><br>
  <input type="checkbox" id="vehicle3" name="vehicle3" value="Boat">
  <label for="vehicle3"> I have a boat</label>
</form>
```

### Submit Button

`<input type="submit">` defines button for submitting the form data to a form-handler.

```html
<form >
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe"><br><br>
  <input type="submit" value="Submit">
</form>

```

### Input Type Reset
reset button that will reset all form values to their default values

```html
<form >
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe"><br><br>
  <input type="submit" value="Submit">
  <input type="reset">
</form>
```
### Input Type Color
is used for input fields that should contain a color a color picker can show up in the input field

```html
<form>
  <label for="favcolor">Select your favorite color:</label>
  <input type="color" id="favcolor" name="favcolor">
</form>
```

#### Input Type Time
`<input type="time">` allows the user to select a time (no time zone).
time picker can show up in the input field.

```html
<form>
  <label for="appt">Select a time:</label>
  <input type="time" id="appt" name="appt">
</form>
```
### Input Type Date
 is used for input fields that should contain a date. a date picker can show up in the input field
we can also use the min and max attributes to add restrictions to dates
``` html
<form>
  <label for="datemax">Enter a date before 1980-01-01:</label>
S
   <input type="date" name="" id="" min="2-13-2023">

   <input type="date" name="" id="" max="1200-12-31">
  
</form>
```
#### Input Type Datetime-local
`<input type="datetime-local">` specifies a date and time input field, with no time zone.
 date picker can show up in the input field.

```html
<form>
  <label for="birthdaytime">Birthday (date and time):</label>
  <input type="datetime-local" id="birthdaytime" name="birthdaytime">
</form>
```

#### Input Type Week
`<input type="week">` allows the user to select a week and year.

date picker can show up in the input field.

```html
<form>
  <label for="week">Select a week:</label>
  <input type="week" id="week" name="week">
</form>
```

### Input Type Month
`<input type="month">` allows the user to select a month and year.

a date picker can show up in the input field.

```html
<form>
  <label for="bdaymonth">Birthday (month and year):</label>
  <input type="month" id="bdaymonth" name="bdaymonth">
</form>
```


#### Input Type Email
`<input type="email"> `is used for input fields that should contain an e-mail address.
e-mail address can be automatically validated when submitted.

```html
<form>
  <label for="email">Enter your email:</label>
  <input type="email" id="email" name="email">
</form>
```
#### Input Type Image
`<input type="image">` defines an image as a submit button.

```html
<form>
<input type="image" src="img_submit.jpg" alt="Submit" width="48" height="48">
</form>
```

### Input Type File
`<input type="file">` defines a file-select field and a "Browse" button for file uploads.

```html
<form>
  <label for="myfile">Select a file:</label>
  <input type="file" id="myfile" name="myfile">
</form>
```
#### Input Type Hidden
`<input type="hidden">` defines a hidden input field (not visible to a user).
hidden field lets web developers include data that cannot be seen or modified by users when a form is submitted.
```html
<form>
  <label for="fname">First name:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <input type="hidden" id="custId" name="custId" value="3487">
  <input type="submit" value="Submit">
</form>
```

#### Input Type Number
`<input type="number">` defines a numeric input field.

we can also set restrictions on what numbers are accepted.


```html
<form>
  <label for="quantity">Quantity (between 1 and 5):</label>
  <input type="number" id="quantity" name="quantity" min="1" max="5">
</form>
```

#### Input Type Range
`<input type="range">` defines a control for entering a number whose exact value is not important (like a slider control). Default range is 0 to 100. However, we can set restrictions on what numbers are accepted with the min, max, and step attributes

```html
<form>
  <label for="vol">Volume (between 0 and 50):</label>
  <input type="range" id="vol" name="vol" min="0" max="50">
</form>
```
#### Input Type Search
`<input type="search">` is used for search fields (a search field behaves like a regular text field).

```html
<form>
  <label for="gsearch">Search Google:</label>
  <input type="search" id="gsearch" name="gsearch">
</form>
```

#### Input Type Tel
`<input type="tel"> `is used for input fields that should contain a telephone number.

```html
<form>
  <label for="phone">Enter your phone number:</label>
  <input type="tel" id="phone" name="phone" pattern="[0-9]{3}-[0-9]{2}-[0-9]{3}">
</form>
```

### Input Type Url
`<input type="url">` is used for input fields that should contain a URL address.

url field can be automatically validated when submitted.

```html
<form>
  <label for="homepage">Add your homepage:</label>
  <input type="url" id="homepage" name="homepage">
</form>
```

## Input Attributes
### Value Attribute
input value attribute specifies an initial value for an input field
```html
<form>
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe">
</form>
```
### Readonly Attribute
input readonly attribute specifies that an input field is read-only.

>A read-only input field cannot be modified (however, a user can tab to it, highlight it, and copy the text from it).


```html
<form>
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John" readonly><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe">
</form>
```
### Disabled Attribute
input disabled attribute specifies that an input field should be disabled.

>disabled input field is unusable and un-clickable.

>value of a disabled input field will not be sent when submitting the form!

```html
<form>
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John" disabled><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe">
</form>
```
### Size Attribute
input size attribute specifies the visible width, in characters, of an input field.

default value for size is 20.
```html
<form>
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" size="50"><br>
  <label for="pin">PIN:</label><br>
  <input type="text" id="pin" name="pin" size="4">
</form>
```
### Maxlength Attribute
input maxlength attribute specifies the maximum number of characters allowed in an input field.

```html
<form>
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" size="50"><br>
  <label for="pin">PIN:</label><br>
  <input type="text" id="pin" name="pin" maxlength="4" size="4">
</form>
```
### Min and Max Attributes
input min and max attributes specify the minimum and maximum values for an input field.
```html
<form>
  <label for="datemax">Enter a date before 1980-01-01:</label>
  <input type="date" id="datemax" name="datemax" max="1979-12-31"><br><br>

  <label for="datemin">Enter a date after 2000-01-01:</label>
  <input type="date" id="datemin" name="datemin" min="2000-01-02"><br><br>

  <label for="quantity">Quantity (between 1 and 5):</label>
  <input type="number" id="quantity" name="quantity" min="1" max="5">
</form>
```
### Multiple Attribute
input multiple attribute specifies that the user is allowed to enter more than one value in an input field.
```html
<form>
  <label for="files">Select files:</label>
  <input type="file" id="files" name="files" multiple>
</form>
```
### Pattern Attribute
input pattern attribute specifies a regular expression that the input field's value is checked against, when the form is submitted.

```html
<form>
  <label for="country_code">Country code:</label>
  <input type="text" id="country_code" name="country_code"
  pattern="[A-Za-z]{3}" title="Three letter country code">
</form>
```
### Placeholder Attribute
input placeholder attribute specifies a short hint that describes the expected value of an input field
```html
<form>
  <label for="phone">Enter a phone number:</label>
  <input type="tel" id="phone" name="phone"
  placeholder="123-45-678"
  pattern="[0-9]{3}-[0-9]{2}-[0-9]{3}">
</form>
```
### Required Attribute
input required attribute specifies that an input field must be filled out before submitting the form.

```html
<form>
  <label for="username">Username:</label>
  <input type="text" id="username" name="username" required>
</form>
```
### Step Attribute
input step attribute specifies the legal number intervals for an input field.

```html
<form>
  <label for="points">Points:</label>
  <input type="number" id="points" name="points" step="3">
</form>
```

### Autofocus Attribute
input autofocus attribute specifies that an input field should automatically get focus when the page loads.
```html
<form>
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" autofocus><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname">
</form>
```
### Height and Width Attributes
input height and width attributes specify the height and width of an `<input type="image">` element.


```html
<form>
  <label for="fname">First name:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <label for="lname">Last name:</label>
  <input type="text" id="lname" name="lname"><br><br>
  <input type="image" src="img_submit.gif" alt="Submit" width="48" height="48">
</form>
```
### List Attribute
input list attribute refers to a `<datalist>` element that contains pre-defined options for an `<input> `element.

```html
<form>
  <input list="browsers">
  <datalist id="browsers">
    <option value="Internet Explorer">
    <option value="Firefox">
    <option value="Chrome">
    <option value="Opera">
    <option value="Safari">
  </datalist>
</form>
```
### Autocomplete Attribute

Autocomplete allows the browser to predict the value. When a user starts to type in a field, the browser should display options to fill in the field, based on earlier typed values.

```html
<form action="/action_page.php" autocomplete="on">
  <label for="fname">First name:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <label for="lname">Last name:</label>
  <input type="text" id="lname" name="lname"><br><br>
  <label for="email">Email:</label>
  <input type="email" id="email" name="email" autocomplete="off"><br><br>
  <input type="submit" value="Submit">
</form>
```
### Name Attribute for `<input>`

Notice that each input field must have a name attribute to be submitted.

If the name attribute is omitted, the value of the input field will not be sent at all.
```html
<form >
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" value="John"><br><br>
  <input type="submit" value="Submit">
</form>
```
### `<select>` Element
`<select>` element defines a drop-down list

```html
<label for="select"> Select Your Favourite Lang </label>
        <select name="" id="select">
            <option value="html">HTML</option>
            <option value="CSS">CSS</option>
            <option value="JavaScript">JavaScript</option>
            <option value="JavaScript">Python</option>
        </select>
```
#### Visible Values:
>Use the size attribute to specify the number of visible values:

#### Option element 
`<option>` elements defines an option that can be selected.

By default, the first item in the drop-down list is selected.

To define a pre-selected option, add the selected attribute to the option:
```html
<option value="fiat" selected>Fiat</option>
```
#### Multiple Selections:
Use the multiple attribute to allow the user to select more than one value

```html

<select name="" id="select" multiple>
            <option value="html">HTML</option>
            <option value="CSS">CSS</option>
            <option value="JavaScript">JavaScript</option>
            <option value="JavaScript">Python</option>
</select>
```
### `<textarea>` Element

`<textarea>` element defines a multi-line input field more space to take user input for text:

```html
<textarea name="message" rows="10" cols="30">
```
`rows `attribute specifies the visible number of lines in a text area.

`cols` attribute specifies the visible width of a text area.

### `<button>` Element
`<button>` element defines a button:

```html
<button type="button" onclick="alert('Hello World!')">Click Me!</button>
```

### `<fieldset>` and `<legend> `Elements

`<fieldset>` element is used to group related data in a form.

`<legend>` element defines a caption for the `<fieldset> `element.

```html
<form >
  <fieldset>
    <legend>Personalia:</legend>
    <label for="fname">First name:</label><br>
    <input type="text" id="fname" name="fname" value="John"><br>
    <label for="lname">Last name:</label><br>
    <input type="text" id="lname" name="lname" value="Doe"><br><br>
    <input type="submit" value="Submit">
  </fieldset>
</form>
```


### <datalist> Element

`<datalist>` element specifies a list of pre-defined options for an `<input>` element.

Users will see a drop-down list of the pre-defined options as they input data.

list attribute of the `<input> `element, must refer to the id attribute of the `<datalist>` element.

```html
<form >
  <input list="lang">
  <datalist id="lang">
   <option value="html">
   <option value="CSS">
   <option value="JavaScript">
   <option value="JavaScript">
  </datalist>
</form>
```

### Form Attributes

Action Attribute 

>action attribute defines the action to be performed when the form is submitted

Usually, the form data is sent to a file on the server when the user clicks on the submit button.

```html
<form action="https://w3schools.com/action_page.php" target="_blank">
```
### Target Attribute

`_blank`	The response is displayed in a new window or tab

`_self`	The response is displayed in the current window

```html
<form action="https://w3schools.com/action_page.php" target="_blank">
```

### Method Attribute

We will Study it latter in backend Modules.

method attribute specifies the HTTP method to be used when submitting form data.

form-data can be sent as URL variables (with method="get") or as HTTP post transaction (with method="post").

default HTTP method when submitting form data is GET. 

```html
<form action="https://w3schools.com/action_page.php" target="_blank" method="post">
```

#### When to Use Get & When to Use Post?

##### Get
NEVER use GET to send sensitive data! length of a URL is limited (2048 characters)
GET is good for non-secure data, like query strings in Google

##### POST
POST is good sending secure data. POST has no size limitations, and can be used to send large amounts of data.

#### Autocomplete Attribute
When autocomplete is on, the browser automatically complete values based on values that the user has entered before

```html
<form action="https://w3schools.com/action_page.php" autocomplete="on">
```

#### Novalidate Attribute

When we use novalidate, it specifies that the form-data (input) should not be validated when submitted.

<form action="https://w3schools.com/action_page.php" novalidate>

