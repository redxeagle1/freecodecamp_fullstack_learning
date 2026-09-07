# general notes

* html is a markup language and it stands for hypertext markup language
* the main role of html is to define the general structure of the website itself and how its layout will be
* the basic building block of the language is tags `<>`

## html tags components

* html tags are written in this general syntax:

```html
<element attribute="value"></element>

```

* and it's not a case-sensitive language (lower and upper case), meaning you can normally mix between cases while writing it, although this is obviously not recommended

### general structure in detail

1. the `<>` at the beginning is called the opening tag and it defines the start of the tag itself and it includes:

* the element: this defines the shape of the element itself and its behavior, whether it's a (heading, button, image, etc.)
* the attribute: this defines the state of the element and its general behavior, and it takes either a `number` or a `string` and here is a simple example:

```html
<a href="https://www.freecodecamp.org/news/" target="_blank">Visit freeCodeCamp</a>

```

* the `<a>` is an element used to put links on text or images, and it has an attribute called `href` which specifies the link you want to put

1. the `</>` is called the closing tag and it defines the end of the tag itself and it only contains the name of the element and nothing else

* obviously i don't need to tell you that tags can be nested or placed inside each other and here an example

```html
<body>

    <!-- Your visible website content goes here -->
    <h1>Hello, World!</h1>

    <p>hey it's me it's <mark> omellete man</mark> he make cookie that no body can</p>
</body>
```

### **important notes**

> 1. not every tag needs a closing tag. for example, the `<img>` tag doesn't need to be closed unless you use a formatting tool like prettier which might do it like this at the end `</img>`, however this is not standard and doesn't do anything
> 2. there is a type of attributes called boolean attributes. these are fixed words or you can consider them basic attributes that define the state of the element. examples include `disabled`, `checked`, and `required`. the names clearly indicate what they do, and keep in mind that if you don't write them, their default value is `false`
