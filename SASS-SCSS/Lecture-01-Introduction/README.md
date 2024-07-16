# Sass Introduction

## Topics Covered:

1. What is SASS/SCSS?
2. Advantages of Using SASS/SCSS Over CSS
3. Setting Up the Environment
4. Basic Syntax and File Structure


## What is Sass?

Welcome to our first lecture on SASS/SCSS! Today, we'll explore what SASS/SCSS is and why it's a powerful tool for web developers. SASS (Syntactically Awesome Style Sheets) is a preprocessor scripting language that is interpreted or compiled into CSS. It provides a more robust, dynamic, and reusable style sheet language."

Sass stands for Syntactically Awesome Stylesheet
Sass is an extension to CSS
Sass is a CSS pre-processor
Sass is completely compatible with all versions of CSS
Sass reduces repetition of CSS and therefore saves time
Sass was designed by Hampton Catlin and developed by Natalie Weizenbaum in 2006
Sass is free to download and use

## Why Use Sass?

Stylesheets are getting larger, more complex, and harder to maintain. This is where a CSS pre-processor can help.

## Advantages of SASS/SCSS

- Variables
- Nesting
- Partials and imports
- Mixins
- Extend/Inheritance

SASS/SCSS offers numerous advantages over plain CSS. These include the use of variables, which allow you to store values that you can reuse throughout your CSS. Nesting lets you write your CSS in a nested hierarchy that follows the same visual hierarchy of your HTML. Partials and imports help you modularize your CSS, making it easier to maintain. Mixins allow you to create reusable chunks of CSS, and @extend lets you share a set of CSS properties from one selector to another

A Simple Example why Sass is Useful
Let's say we have a website with three main colors:

```#a2b9bc```

```#b2ad7f```

```#878f99```

So, how many times do you need to type those HEX values? A LOT of times. And what about variations of the same colors?

Instead of typing the above values a lot of times, you can use Sass and write this:

Sass Example

```$primary_1: #a2b9bc;```
```$primary_2: #b2ad7f;```
```$primary_3: #878f99;```

```css
.main-header {
  background-color: $primary_1;
}
.menu-left {
  background-color: $primary_2;
}

.menu-right {
  background-color: $primary_3;
}
```

So, when using Sass, and the primary color changes, you only need to change it in one place.

## How Does Sass Work?

A browser does not understand Sass code. Therefore, you will need a Sass pre-processor to convert Sass code into standard CSS.

This process is called transpiling. So, you need to give a transpiler (some kind of program) some Sass code and then get some CSS code back.

Tip: Transpiling is a term for taking a source code written in one language and transform/translate it into another language.

### Sass File Type

Sass files has the ".scss" file extension.

### Comment in SCSS

Sass supports standard CSS comments ```/* comment */```, and in addition it supports inline comments ```// comment```:

Sass Example defining variables.
```/* define primary colors */```

```css
$primary_1: #a2b9bc;
$primary_2: #b2ad7f;
```

### use the variables

```css
.main-header {
  background-color: $primary_1; // here you can put an inline comment
}
```

## Setting Up the Environment

- Install Node.js and npm
- Install SASS using npm: npm - - install -g sass
- Alternative: Standalone SASS - installer link
- Basic project structure example

to get started with SASS, you'll need to set up your environment. First, make sure you have Node.js and npm installed on your computer. Once you have those, you can install SASS globally using npm with the command npm install -g sass. Alternatively, you can download and install a standalone version of SASS from the official website. Let's set up a basic project structure together.

## Basic Syntax and File Structure

```scss
Variables: $primary-color: #333;
Nesting: .nav { .nav-item { color: $primary-color; } }
```

File structure: styles.scss, styles.css
my-sass-project/
├── styles.scss
└── styles.css

"SASS/SCSS syntax is very similar to CSS, with a few additional features. Variables start with a $ sign, and you can nest your CSS rules to mirror the structure of your HTML. Let's look at a simple example."SASS/SCSS syntax is very similar to CSS, with a few additional features. Variables start with a $ sign, and you can nest your CSS rules to mirror the structure of your HTML. Let's look at a simple example.


"That's it for our first lecture on SASS/SCSS. We've covered the basics of what SASS/SCSS is, its advantages over CSS, how to set up the environment, and some basic syntax. Do you have any questions? Feel free to ask! For further reading, check out the official SASS documentation and tutorials linked on the slide."

### Resources:
- **SASS Official Documentation:** [https://sass-lang.com/documentation](https://sass-lang.com/documentation)
- **Node.js and npm Installation Guide:** [https://nodejs.org/en/download/](https://nodejs.org/en/download/)