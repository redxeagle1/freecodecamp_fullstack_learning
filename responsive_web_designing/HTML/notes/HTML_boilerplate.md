# HTML boilerplate

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="./styles.css" />
</head>
<body>

</body>
</html>
```

- Importances :
  - It ensures your pages are structured correctly and work well across different browsers.
  - Using a boilerplate helps you avoid common mistakes and follow best practices.
  - It's a great starting point for any web project.

> Remember, you can customize your own boilerplate to fit your needs. As you gain experience you might add your own preferred elements or `<meta>` tags.

## HTML link element

- the `<link>` element is used to link to external resources like stylesheets icons and fonts like linking your stylesheet
- relationship between the linked resource and the HTML document example using it

```html
<link rel="stylesheet" href="./styles.css" />
```

another one is

```html
<link rel="icon" href="favicon.ico" />
```

> A favicon, which is short for favorite icon, is a small icon typically displayed in the browser tab next to the site title. A lot of websites will use a favicon to display their brand icon.

- attributes
  - `rel` which is used to specify the relationship between the linked resource and the HTML document here is some example
    - `stylesheet` value specifies that the linked resource is a css file
    > it's a best practise not to dump your css javascript and html inside a single file instead you should always seperate your file
    - `preconnect` value tells the browser to create an early connection to the value specified in the `href` attribute. This is done to speed up loading times for these external resources.
  - `href` attribute is used to specify the location of the URL for the external resource. whether it's a path or url
    - like telling the location or the url of a font or icons

- it's a ready-made template for your webpages. it includes the basic structure and essential elements every HTML document needs.

## boilerplate breakdown

1. `<!DOCTYPE html>` It tells browsers which version of HTML you're using.
2. `<html>...content...</html>` This wraps around all your content and can specify the language of your page
   - inside it you will finde the `<head>` and the `body` elements
3. `<head>...content..</head>` contains important behind-the-scenes information like:
   1. `<meta>` has details about things like character encoding, and how websites like Twitter should preview your page's link. one of its important attribute are
      - `charset` : which defines youe character encoding ,method computers use to store characters as data
       Essentially, all text on a web page is a sequence of characters stored as one or more bytes
       > `UTF-8` supports every character in the Unicode character set, and this includes characters and symbols from all writing systems, languages, and technical symbols. For each new project you create, ***you should include this meta element with the `charset` attribute set to `UTF-8`.***
   2. `<title>` which determines the text that appears in the browser tab or window
   3. `<link>` whiich we discussed earlier
4. `<body>...content..</body>` section is where all your content goes
