# intro

- SEO, or Search Engine Optimization, is a practice that optimizes web pages so they become more visible and rank higher on search engines.

## Role of the Meta Description

- using the `meta` element to provide a short description for the web page using the as the following example

    ```html
    <meta
    name="description"
    content="Discover expert tips and techniques for gardening in small spaces, choosing the right plants, and maintaining a thriving garden."
    />
    ```

    > Setting the `name` attribute to `"description"` ensures that browsers, search engines, and other web tools correctly interpret this metadata.
    > the `content` attribute is where you will place your `"description"`. It is recommended that you keep your `"descriptions"` short and concise. This is because search engines **will often truncate the** `"description"` based on the results page layout.

### Open Graph Tags aka OG

- The open graph (og) protocol enables you to control how your website's content appears across various social media platforms, such as Facebook, LinkedIn, and many more.
- You can set these (og) properties through a collection of meta elements inside your HTML head section.

- **How Open Graph Properties Affect Search Engine Optimization?**
  - When your content is shared on social media, well-crafted OG properties can enhance the appearance for your content in users' feeds. This can lead to higher click-through rates, which could signal to search engines that your content is relevant and engaging.

- OG properties

  1. `title` Here is an example of setting the OG title for the freeCodeCamp homepage:

      ```html
      <meta content="freeCodeCamp.org" property="og:title" />
      ```

      > The `content` attribute is where you will write the title you want displayed for social media sites.
      > For the `property` attribute, you will need to specify that it is `og:title`.
  2. the `type` Here is an example of using the OG type for the freeCodeCamp homepage:

      ```html
      <meta property="og:type" content="website" />
      ```

      > The `type` property is used to **represent the type of content being shared** on social media. Examples of this content include `articles`, `websites`, `videos`, or `music`.
  3. the `image` Here is an example of setting the OG image for the freeCodeCamp homepage:

      ```html
      <meta
        content="<https://cdn.freecodecamp.org/platform/universal/fcc_meta_1920X1080-indigo.png>"
        property="og:image"
      />
      ```

      > In this example, the OG `image` is pointing to the freeCodeCamp logo.

      - All of these images should be high quality with good dimensions and ratios. Most social media platforms will include criteria for image requirements <!-- markdownlint-disable-line MD007 -->
      - use images that are at least 1200 by 630 pixels for the best display on high resolution devices. At the minimum, you should use images that are 600 by 315 pixels to display link page posts with larger images <!-- markdownlint-disable-line MD007 -->
  4. the `url`. Here is an example of setting the OG `url` for the freeCodeCamp homepage:

      ```html
      <meta property="og:url" content="https://www.freecodecamp.org" />
      ```

> There are many more OG properties that you can set, like description, audio, video and locale. However, the open graph url, image, type, and title are the most important ones to include.

## HTML5 tag best practices

- HTML5 has some elements that identify different content areas. These elements make your HTML easier to read and help with Search Engine Optimization (SEO) and accessibility.

- The `<main>` element is used to represent the main content of the body of an HTML document. Content inside the main element ***should be unique to the document and should not be repeated*** in other parts of the document.

- The `<section>` element is used to define sections in a document, such as chapters, headers, footers, or any other sections of the document.***It is a semantic element that helps with SEO and accessibility.***

- The `<footer>` element is used to define a footer for a document or section. A footer typically contains
  - information about the author of the document
  - copyright data
  - links to terms of use
  - contact information, and more.
