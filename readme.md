# HTML:
## Working of HTML:
* An external web server stores your HTML files and sends them to a user's web browser over the internet when requested
* On an external server:
    The Request: You type a website address into your browser. Your browser sends an HTTP request across the internet to the external server's IP address.
    The Lookup: The server receives the request, looks in its storage folders for the requested HTML file (such as index.html), and prepares a reply.
    The Response: The server sends the raw HTML text back to your browser with a success status code (like 200 OK).
    The Rendering: Your browser reads the incoming HTML code and turns it into the visual webpage you see on your screen.
    Loading Extra Files: If your HTML links to other files like CSS stylesheets, JavaScript, or images, your browser sends separate, follow-up requests to the server to grab those pieces.
```html
    http://    localhost    :3000    /assets/styles.css    ?theme=dark
  ──┬──    ────┬────    ──┬──    ────────┬─────────    ─────┬─────
    │         │         │              │                 └── Query Parameters
    │         │         │              │                     (Data sent to server)
    │         │         │              └── Pathname 
    │         │         │                  (Target file system structure)
    │         │         └── Port Number 
    │         │             (Directs traffic to your specific dev tool)
    │         └── Hostname 
    │             (Mapped internally by your computer to IP 127.0.0.1)
    └── Protocol/Scheme 
        (Usually unencrypted HTTP during development)

```

## HTML Document Format:

### Document type Declaration:

This statement tells the web browser what versin of HTML the document is written in.It helps the browser interpret and display the code correctly.
`<!DOCTYPE html>`

### HTML Tag:

It is the starting point or the main container of the webpage.It is like the root or base of a tree which other elements are branch out.All the text,images and links is nested with this HTML Tag.
`<html>`

### Head:

The head section is like a store room for important details about the webpage,such as its title,design,instructions and extra features.It contains the background information that helps the webpage function correctly and look good.
`<head></head> `

### Body:

the body section of a webpage is where you find all the main content like text,images,headings,and lists.

## 1_Elements of HTML:

```html
  <!DOCTYPE html> 
  This declaration defines that the document is an HTML5 document. It must always be the very first line of your code. 
  <html>...</html> 
  This is the root element of the page. All other elements are nested inside it. 
  <head>...</head> 
  The <head> section contains meta-information that isn't displayed directly on the page, like the page title or links to CSS stylesheets. 
  <title>...</title> 
  The <title> tag sets the title of the webpage. This is what you see in the browser tab and what search engines use as the main title in search results. 
  <body>...</body> 
  The <body> tag contains all the visible content of your webpage—headings, paragraphs, images, links, etc. 

```

### Essential HTML Elements:

Elements are the building blocks of HTML. These are the tags that can we used everyday.

#### Basic

```html
 <h1> to <h6>     Defines HTML headings
 <p>     Defines a paragraph
 <br>     Inserts a single line break
 <hr>     Defines a thematic change in the content
 Defines a comment

```

#### Formatting

```html
<b> - Bold text
<strong> - Important text
<i> - Italic text
<em> - Emphasized text
<mark> - Marked text
<small> - Smaller text
<del> - Deleted text
<ins> - Inserted text
<sub> - Subscript text
<sup> - Superscript text

```

#### Forms and links

```html
<form>     Defines an HTML form for user input
<input>     Defines an input control
<textarea>     Defines a multiline input control (text area)
<button>     Defines a clickable button
<select>     Defines a drop-down list
<optgroup>     Defines a group of related options in a drop-down list
<option>     Defines an option in a drop-down list
<label>     Defines a label for an <input> element
<fieldset>     Groups related elements in a form
<legend>     Defines a caption for a <fieldset> element
<datalist>     Specifies a list of pre-defined options for input controls
<output>     Defines the result of a calculation.
<a>     Defines a hyperlink
<link>     Defines the relationship between a document and an external resource (most used to link to style sheets)
<nav>     Defines navigation links

```

## 2_Attributes:

* All HTML elements can have attributes
* Attributes provide additional information about elements
* Attributes are always specified in the start tag
* Attributes usually come in name/value pairs like: name="value"

`Eg: <a href="https://www.google.com">Visit Google</a>`

### href attribute:

```
<a> tag defines a hyperlink. Then href specifies the URL of the page that goes 

```

### src attribute:

```
<img> tag is used for embed an image in an HTML page. src represents the path to the image to be displayed. 

```

`<img src="img_sample.jpeg"> `

#### url can be displayed in two ways:

**Absolute URL:** Links an external image that is hosted on another website
eg:
`src=”https://static.wixstatic.com/media/2b9330_dd668a2e1d664129a64eba0689ffd142~mv2_d_1920_1386_s_2.jpg/v1/fill/w_560,h_374,al_c,q_80,usm_0.66_1.00_0.01,enc_avif,quality_auto/africa-animal-big-cat-88234.jpg” `
Note: by using the external links might be under copyright. If you do not get permission to use it, you may be in violation of copyright laws. In addition, you cannot control external images; it can suddenly be removed or changed.

**Relative URL:** Links to an image that is hosted in within the website
`Eg: src=”image_sample.png” `

Note : always best to use relative URLs.This will  not affect any webpages.

### Width and height attributes:

Image tag also contain the width and the height tags that can be used for adjusting the height and width of the image.

`Eg:<img src=”img_sample.jpg” height=”200px” width=”300px”>`

### Alt attributes:

```
Alt attributes can be used in the situation of whether the image is not displayed on the webpage 
Eg: when the image is in the absolute url and there’s no internet connection means then the altenative text content can be displayed. 
`<img src=”img_sample.jpg” alt="sample image" height=”200px” width=”300px”>` 

```

### Style attribute:

The style attribute is used to add styles to an element, such as color, font, size, and more.
Eg:It can be used for the inline css.
`<p style="color:red;">This is a paragraph</p>`

### Lang attribute:

Lang attribute mentions the language of the webpage which is inside the html tag.

```html
<!DOCTYPE html>
<html lang="en">

```

### The title Attribute

The title attribute defines some extra information about an element.
The value of the title attribute will be displayed as a tooltip when you mouse over the element
`<p title="This is a tooltip">This is a pararaph</p>`

## 3_Head tags  to :

HTML provides the 6 levels of headings  is the most important  is the least important.
Search engines use the headings to index the structure and content of your web pages.
Users often skim a page by its headings. It is important to use headings to show the document structure.

For example:
`<h1>` - Page title
`<h2>` - Section titles
`<h3>` - Sub-sections

Each heading has a default  size details. We can specify the size by using the style attribute.

## 4_Paragraph tags:

A tag starts on a new line and browsers automatically add some white space before and after the paragraph.

```html
Note: 
Eg:  
<p> This is a paragraph.This one is the line</p> 
<p>This is another paragraph</p>.This works 
<p>This is one paragraph 

```

This is another.This doesn’t works because the  tag automatically remove the whitespace from the browser. This is the poem problem.
To overcome this, we can use the  tag

### Pre Tag:

The HTML  element defines preformatted text.
The text inside a  element is displayed in a fixed-width font (usually Courier), and it preserves both spaces and line breaks

## 5_Styles:

Style attribute is used to add styles to an element such as color,font size,and more;
Syntax:
`<tagname style=”property:value;”>`
Within style attribute we can build the inbuilt css features.

### Background color:

It defines the background-color of a n HTML element.

### Text color:

Color property defines the text color of an HTML element.

### Fonts:

Font-family property defines the font to be used for an HTML element.

### Text Size:

CSS font-size defines the text size for a HTML element.

### Text Alignment:

CSS text-align defines the horizontal text alignment for an HTML element.

## 6_Quotation and Citation Elements

`   <blockquote>,<q>,<abbr>,<address>,<cite>,<bdo>`

`<blockquote cite="https://localhost:300">Here's a sample blockquote paragraph which can be intended.It can be quoted from another source</blockquote>`
  short quoted text
it is used for short quotation
Browsers usually insert the quotation marks for the short quotes.

`<q>This is a short quoted text</q>`

```
<abbr>abbrevation quotes
it is used for the full form of the words.

```

`<p>The <abbr title="World Health Organization">WHO</abbr> released a new artile about the recent war</p>`

```
<address> it is used for contact information  like address,mobile number and email

```

`<address>Written and mentioned by<br>The author,and their team<br>The book name,<br>location address</address>`

```
<cite> mentions the title of a creative work(book,poem,song,movie,painting,sculpture etc) not the person.

```

it usually renders in italic.
`<p>The <cite>book</cite> which was written by the author was published successfully</p> `

```
<bdo> Bidirectional Override
Override the current text direction.

```

`<bdo dir="rtl">This is a reversed text</bdo>`

## 7_Text Formatting:

Formatting is used to display special types of text

```html
  <b> - Bold text 
  <strong> - Important text 
  <i> - Italic text 
  <em> - Emphasized text 
  <mark> - Marked text 
  <small> - Smaller text 
  <del> - Deleted text 
  <ins> - Inserted text 
  <sub> - Subscript text 
  <sup> - Superscript text

```

### The difference between the `<b>` and `<strong>`:

```
<b> defines the text without any importance . 
<strong> it shows with strong importance .The content also displayed in bold. 

```

### Where we use  tag:

For  making the bold text in headings .Eg: **Topic1**

### Where we use  tag:

```
For mentioning the importantance of word in a text. 

```

**Eg: This conversation is highly confidential.**
 ### Difference between the `<i>` and `<em>` tags:
The HTML  element defines a part of text in an alternate voice or mood. The content inside is typically displayed in italic.
Tip: The  tag is often used to indicate a technical term, a phrase from another language, a thought, a ship name, etc.
`Eg:     <i>This text is italic</i>`

The HTML  element defines emphasized text. The content inside is typically displayed in italic.
Tip: A screen reader will pronounce the words in  with an emphasis, using verbal stress.
Eg:  `<em>This text is emphasized</em>`

```html
  <small>- makes the text smaller 
  <mark > makes the text marked and highlighted 
  <del> the selected text be individually deleted 
  <ins> defines a text that has been inserted into the document 
  <sub> element defines subscript text. Subscript text appears half a character below the normal line, and is sometimes rendered in a smaller font.  
  Eg: Subscript text can be used for chemical formulas, like H2O 
  <sup> element defines superscript text. Superscript text appears half a character above the normal line, and is sometimes rendered in a smaller font.  
  Eg: Superscript text can be used for footnotes, like WWW[1]

```

## 8_HTML Comment Tag:

We can add comments to your HTML source by using the following syntax:
``

Note1: that there is an exclamation point (!) in the start tag, but not in the end tag.
Note2: Comments are not displayed by the browser, but they can help document your HTML source code.

## 9_Colors
  can be applied to text,borders and backgrounds
  forms,links,tables etc..
  colors can be applied by various forms.
    RGB
    HEX
    HSL
    HSLA
    RGBA
  background-color
  color
  border
  why decimal values are used in RGB:
  decimal values are easily unserstandable for humans and easy to calculate
  human redability
  mapping to bytes
    computers store each color channel in 8 bits an hold 2^8 (256) different values ranging from 0 to 255
  Alpha channel support shorthand hex codes cannot easily show opacity
  using decimal notation shows the clear decimal fraction directly into the code
  RGB
    red green blue(in a decimal form)
    0 to 255 values
    These 3 color values are mixed to get the actual color
  RGBA
    A-alpha
    can be used for color transparency
    it can be started from 0 to 1.0
    0.5 s the semi transparency
  HEX
    are specified by combinig the hexadecimal values of red green and blue 
    with each value ranging from 00 to ff
    00 represents the lower intensity
    ff represents the higher intensity
    value starts with the # sign and includes six digits(##RRGGBB)
  HSL
    a color can be specified using hue,saturation and lightness
    hue is a degree on the color wheel from 0to 360
    red s 0,120 is green 240 is blue
    sauration is percentage value
    0% is a shade of grey
    100% is full color
    Lightness is also a percentage 0% is black and 100% is white
  HSLA
    comes with an alpha channel
    0.0 fully transparent and 1.0 no transparent 
  **Here are the various color values used on the text**
```html
       <h1>Font color and color values</h1>
        <h2 style="color:tomato;">This heading applies the direct color Name</h2><!--direct color-->
        <p style="color:rgb(40, 145, 132)">This paragraph uses the rgb color values</p><!--rgb color-->
        <p style="color:rgba(40,145,132,0.5)">This paragraph uses the rgba color values</p><!--rgba color-->
        <p style="color:#553496">This text is using the HEX color values</p><!--hex color-->
        <pre style="color:hsl(32, 70%, 59%);">This text is using the hsl color values</pre><!--hsl color-->
        <pre style="color:hsla(32, 70%, 59%,0.5);">This text is using the hsla color values</pre><!--hsla color-->
```
## 10_HTML CSS Styles:

Css can be used to format the layout of a webpage.
With CSS, you can control the color, font, the size of text, the spacing between elements, how elements are positioned and laid out, what background images or background colors are to be used, different displays for different devices and screen sizes, and all..
Using CSS
CSS can be added to HTML documents in 3 ways:

* Inline - by using the style attribute inside HTML elements
* Internal - by using a  element in the  section
* External - by using a  element to link to an external CSS file

The most common way to add CSS, is to keep the styles in external CSS files. However, in this tutorial we will use inline and internal styles, because this is easier to demonstrate, and easier for you to try it yourself.

### Inline CSS

An inline CSS is used to apply a unique style to a single HTML element.
It uses the style attribute of an HTML element.
Eg: it sets the text color of the  element to blue, and the text color of the  element to red.

```html
  <h1 style="color:blue;">A Blue Heading</h1> 
  <p style="color:red;">A red paragraph.</p>

```

### Internal CSS

An internal CSS is used to define a style for a single HTML page.It is defined in the  section of an HTML page, within a  element.
Eg: we can set the text color of ALL the  elements (on that page) to blue, and the text color of ALL the  elements to red. In addition, the page will be displayed with a "powderblue" background color.

```html
  <style> 
  body {background-color: powderblue;} 
  h1   {color: blue;} 
  p    {color: red;} 
  </style> 
  <h1>This is a heading</h1> 
  <p>This is a paragraph.</p>

```

### External CSS

An external style sheet is used to define the style for many HTML pages.
To use an external style sheet, add a link to it in the  section of each HTML page:
Eg:

```html
  <head><link rel="stylesheet" href="styles.css"></head> 
  <h1>This is a heading</h1> 
  <p>This is a paragraph.</p> 
  "styles.css": 
  body { 
    background-color: powderblue; 
  } 
  h1 { 
    color: blue; 
  } 
  p { 
    color: red; 
  } 

```

#### CSS Color,Font-size,Font –family:

```
 color property defines the text color to be used. 
 font-family property defines the font to be used. 
 font-size property defines the text size to be used. 

```

For implementation refer the styles topic

#### CSS Border

```
The CSS border property defines a border around an HTML element. 
Note: we can define a border for nearly all HTML elements. 

```

`Eg:   p {border: 2px solid powderblue;} `

### CSS Padding

```
The CSS padding property defines a padding (space) between the text and the border. 
Eg: 

```

```html
  p { 
    border: 2px solid powderblue; 
    padding: 30px; 
  }  

```

### CSS Margin

```
The CSS margin property defines a margin (space) outside the border. 
Eg: 

```

```html
  p { 
    border: 2px solid powderblue; 
    margin: 50px; 
  }  

```

**Relation between Margin and Padding and Border**

```html
  +-----------------------------------------------------------+
  |                         MARGIN                            |
  |     (Creates space between this element and others)       |
  |  +-----------------------------------------------------+  |
  |  |                      BORDER                         |  |
  |  |    (The visible outline around the element)         |  |
  |  |  +-----------------------------------------------+  |  |
  |  |  |                   PADDING                     |  |  |
  |  |  |    (Creates space between border and content) |  |  |
  |  |  |  +-----------------------------------------+  |  |  |
  |  |  |  |                 CONTENT                 |  |  |  |
  |  |  |  |        (Text, images, etc.)             |  |  |  |
  |  |  |  +-----------------------------------------+  |  |  |
  |  |  +-----------------------------------------------+  |  |
  |  +-----------------------------------------------------+  |
  +-----------------------------------------------------------+

```

#### Link to External CSS

External style sheets can be refered with a full URL or with a path relative to the current web page.

## 11_HTML LINKS

### Text Links:

HTML links are hyperlinks.
You can click on a link and jump to another document.
When you move the mouse over a link, the mouse arrow will turn into a little hand.
By default, links will appear as follows in all browsers:
An unvisited link is underlined and blue
A visited link is underlined and purple
An active link is underlined and red
`<a href="https://www.google.com>Click for google</a>`
By default, the linked page will be displayed in the current browser window. To change this, you must specify another target for the link.
The target attribute specifies where to open the linked document.
The target attribute can have one of the following values:
_self - Default. Opens the document in the same window/tab as it was clicked
_blank - Opens the document in a new window or tab
_parent - Opens the document in the parent frame
_top - Opens the document in the full body of the window
`html <a href="[https://www.google.com](https://www.google.com)" target="_self">Click for google!!!</a><br><a href="[https://www.stackoverflow.com](https://www.stackoverflow.com)" target="_parent">Click for stack overflow!!</a><br><a href="[https://www.google.com](https://www.google.com)" target="_top">Click for google!!!</a>  <br><a href="[https://www.google.com](https://www.google.com)" target="_blank">Click for google!!!</a>  <br>`

### Security with rel Attribute

When you open links in new tabs using target="_blank", you need to add a security measure. Without it, the new page could potentially access your original page and cause problems.
The rel="noopener noreferrer" attribute prevents the new page from accessing your original page. Always include this when using target="_blank"
**noopener:** Prevents the new page from accessing the window object of your original page. This stops potential security exploits.
**noreferrer:** Prevents sending referrer information to the new page. This adds privacy by not telling the destination site where the visitor came from.
`<a href="https://www.google.com" target="_blank" rel="noopener noreferrer">Click for google safely!!!</a>  <br>`

### Use Image as a link:

```
To use an image as a link, just put the <img> tag inside the <a> tag:
`       <a href="https://medium.com"><img src="\gif_image.gif" alt="mushroom image"/></a>`

```

Here are some example codes that explain the usage of image links in HTML:

* Create Hyperlink for an Image
* Image Link with Tooltip
* Mouse-Sensitive Images
* Server-Side Image Maps
* Client-Side Image Maps
Image link with tooltip:
You can also define a tooltip for an image link; when someone moves the mouse over the linked image, it will display a tooltip. To set the tooltip, you can set the title attribute of the  tag.
`<a href="https://medium.com" title="go to medium"><img src="\gif_image.gif" alt="mushroom image"/></a>`
#### Mouse sensitive images:
HTML provides a feature that embed the different types of links in the single image then we can add the different links based on the co ordinates.such mouse sesitive images are known as image maps.
In image maps there are  two types:
Server-side image maps: This is enabled by the ismap attribute of the  tag and requires access to a server and related image-map processing applications.
Client-side image maps: This is created with the usemap attribute of the  tag, along with corresponding  and  tags.
In HTML, ismap and usemap are attributes used to create image maps, which turn an image into a set of multiple clickable links or regions. The core difference comes down to where the processing happens: ismap works on the server side, while usemap works on the client side (the browser).


```html
<br><p>with usemap</p>
<br><img src="\gif_image.gif" usemap="#shape-map" alt="Interactive Shapes">
<map name="shape-map">
<area shape="rect" coords="34,44,270,350" href="[https://www.google.com](https://www.google.com)" alt="Rectangle Page">
<area shape="circle" coords="450,200,60" href="[https://www.medium.com](https://www.medium.com)" alt="Circle Page">
</map><br> <p>with ismap</p>
<br><a href="[https://medium.com](https://medium.com)"><img src="\gif_image.gif" ismap alt="mushroom image"/></a><br>```


```



### HTML Email Links:

HTML email links allow users to click on a link and automatically open their default email client with a new message composed to the specified email address.
This is done using the mailto: protocol in the href attribute of an  (anchor) tag.
we can also predefine the subject and body of the email using the mailto: protocol.
This is done by appending ?subject= and &body= to the email address. Spaces and special characters in the subject and body should be URL-encoded.
For example, spaces are encoded as %20.
`html <a href="mailto:example@example.com?subject=Hello%20there&body=This%20is%20a%20predefined%20email%20body.">  Click here to Send Mail</a>`

```
  Cons
      Adding an HTML email link to your webpage can expose your email address to spam. Automated programs, known as email harvesters, can scan web pages for email addresses and add them to spam lists.
       This can result in a significant increase in unwanted emails.

```

## 12_HTML Image tag:

* The HTML  tag is used to embed an image in a web page.
* Images are not technically inserted into a web page; images are linked to web pages. The  tag creates a holding space  for the referenced image.
* The  tag is empty, it contains attributes only, and does not have a closing tag.
* The  tag has two required attributes:
* src - Specifies the path to the image
* alt - Specifies an alternate text for the image
Syntax :
`<img src="url" alt="alternatetext">`
The attributes like src,alt,height and width are mentioned on the attributes topic.
We can also add the gif formated images on the web by using web server.
### Images in Another Folder:


If you have your images in a sub-folder, you must include the folder name in the src attribute:
Example
`<img src="/images/html5.gif" alt="HTML5 Icon" style="width:128px;height:128px;">`

## 13_Favicon
 * It is a small-sized image that displays in the browser's tab just before the page title. 
 * Favicon is defined by using the `<link>` tag with the "rel=icon" attribute.
 ```json
 FaviconDimension 	Used For
  32x32    	        Desktop Browsers
  57x57             Mac ios
  76x76   	        Apple ipad
  96x96 	          Google TV
  120x120 	        Iphone Retina Touch Screen
  128x128 	        Chrome Web Store, Windows 8* Screen
  144x144 	        Internet Explorer 10 Metro
  152x152 	        Apple Ipad
  167x167 	        Apple Ipad
  180x180 	        Apple Iphones
  192x192 	        Google Developer Apps
  195x195 	        Opera Speed Dial
  196x196 	        Android Home of Chrome
  228x228 	        Opera Cast Icon
 ```
 **Syntax**
 `<link rel="icon" href="logo.jpg" type="image/x-icon">`

  ### How To Add a Favicon in HTML
  You can add a favicon to a webpage by using the `<link>` tag with the rel attribute set to "icon". The `<link>` tag is a head element, so it must be placed within the `<head>` tag.
## 14_Tables
  HTML tables represent data, such as text, images, etc. in a structured format with rows and columns.
  HTML tables offer a visual structure that aids in clarity and comprehension, making them a fundamental element in web development.
  You can create a table in HTML by using the `<table>` tag along with several tags that define the structure and content inside the table. The primary tags that are used with the `<table>` tag are `<tr>`, `<td>`, and `<th>`.
  Creating tables in HTML involves several elements that define the structure and content. The primary tags used are `<table>`, `<tr>`, `<td>`, and `<th>`.
    HTML `<table>` Tag: This tag is used to create the table that wrap the rows and columns within it.
    HTML `<tr>` Tag: Stands for "table row" and is used to create a row within the table.
    HTML `<td>` Tag: Represents "table data" and is used to create standard cells within a row.
    HTML `<th>` Tag: Represents "table header" and is used to create header cells within a row.
  Styling HTML Tables
  You can also style an HTML table using CSS properties to give it a custom appearance. Either you can create classes to apply styles on a table, or you can simply write internal CSS properties to style the table.
```html
<head>
   <style>
   table {
      width: 100%;
      border-collapse: collapse;
      margin-bottom: 20px;
   }
   th, td {
      border: 1px solid #ddd;
      padding: 8px;
      text-align: left;
   }
   th {
      background-color: #f2f2f2;
   }
   </style>
</head>
<body>
    <h2>HTML Table</h2>
    <p>This table includes table header.
    <table>
        <tr>
           <th>Header 1</th>
           <th>Header 2</th>
           <th>Header 3</th>
        </tr>
        <tr>
           <td>Data 1</td>
           <td>Data 2</td>
           <td>Data 3</td>
        </tr>
        <tr>
           <td>Data 4</td>
           <td>Data 5</td>
           <td>Data 6</td>
        </tr>
    </table>
  <body>
```
Colspan
To make a cell span over multiple columns, use the colspan attribute
```html
<table>
  <tr>
    <th colspan="2">Name</th>
    <th>Age</th>
  </tr>
  <tr>
    <td>xxx</td>
    <td>yyy</td>
    <td>43</td>
  </tr>
  <tr>
    <td>aaa</td>
    <td>zzz</td>
    <td>57</td>
  </tr>
</table>
```
Rowspan
To make a cell span over multiple rows, use the rowspan attribute
```html
<table>
  <tr>
    <th>Name</th>
    <td>Jill</td>
  </tr>
  <tr>
    <th rowspan="2">Phone</th>
    <td>123456789</td>
  </tr>
  <tr>
    <td>987654321</td>
</tr>
</table>
```
### Colgroup
The <colgroup> element should be used as a container for the column specifications.
Each group is specified with a <col> element.
The span attribute specifies how many columns get the style.
The style attribute specifies the style to give the columns.

```html
<head>
<style>
table, th, td {
  border: 1px solid black;
  border-collapse: collapse;
}
</style>
</head>
<body>

<h2>Colgroup</h2>
<p>Add the a colgroup with a col element that spans over two columns to define a style for the two columns:</p>

<table style="width: 100%;">
<colgroup>
  <col span="2" style="background-color: #D6EEEE">
</colgroup>
<tr>
<th>MON</th>
<th>TUE</th>
<th>WED</th>
<th>THU</th>
<th>FRI</th>
<th>SAT</th>
<th>SUN</th>
</tr>
<tr>
<td>1</td>
<td>2</td>
<td>3</td>
<td>4</td>
<td>5</td>
<td>6</td>
<td>7</td>
</tr>
<tr>
<td>8</td>
<td>9</td>
<td>10</td>
<td>11</td>
<td>12</td>
<td>13</td>
<td>14</td>
</tr>
<tr>
<td>15</td>
<td>16</td>
<td>17</td>
<td>18</td>
<td>19</td>
<td>20</td>
<td>21</td>
</tr>
<tr>
<td>22</td>
<td>23</td>
<td>24</td>
<td>25</td>
<td>26</td>
<td>27</td>
<td>28</td>
</tr>
</table>

</body>
```

## 15_Lists
  HTML lists are group or collection of items. These items can be both organized and unorganized depending on the requirement. They help in organizing, structuring, and presenting information to make it more user-friendly, readable, and accessible
  ordered, unordered, and definition lists
  All lists must contain one or more list elements.
  ### Unordered Lists
  display lists of items that are not in a specific order
  lists are marked with bullet points
  `<ul>` tag is used along with the `<li>` tag
  `<li>` mentions list items
```html
  <ul>
      <li>HTML</li>
      <li>CSS</li>
      <li>JavaScript</li>
      <li>Java</li>
      <li>JavaFX</li>
   </ul>
```
  ### Ordered Lists
   items that are in a specific order. 
   lists are marked with numbers by default
   you can change the numbers into alphabets, roman numbers, etc. 
   by using the type attribute or the CSS list-style-type property
  `<ol>` tag is used along with the `<li>` tag
```html
 <ol>
      <li>HTML</li>
      <li>CSS</li>
      <li>JavaScript</li>
      <li>Java</li>
      <li>JavaFX</li>
   </ol>
```
  ### Definition Lists
  lists of items with their corresponding descriptions.
  The definition lists are created by using the `<dl>`, `<dt>`, and `<dd>` tags.
  Where the `<dl>` tag specifies the "definition list", the `<dt>` tag specifies the "definition term", and the `<dd>` tag specifies the "definition description".
```html
 <dl>
        <dt>HTML</dt>
        <dd>HyperText markup languague</dd>
        <dt>CSS</dt>
        <dd>Cascading Style Sheet</dd>
        <dt>JS</dt>
        <dd>JavaScript</dd>
    </dl>
```
  ### Nested Lists
  within another list is known as a nested list
## 16_Block and Inline Elements
  Every HTML element has a default display value, depending on what type of element it is.
  The two most common display values are block and inline.
 ### Block-level Elements
  A block-level element always starts on a new line, and the browsers automatically add some space (a margin) before and after the element.
  A block-level element always takes up the full width available (stretches out to the left and right as far as it can).
  Two commonly used block elements are: `<p>` and `<div>`.
  The `<p>` element defines a paragraph in an HTML document.
  The `<div>` element defines a division or a section in an HTML document.

  The `<p>` element is a block-level element.
  The `<div>` element is a block-level element.
  ```html
  <p>Hello World</p>
  <div>Hello World</div>
  ```
 ### Inline Elements
  An inline element does not start on a new line.
  An inline element only takes up as much width as necessary.
  This is a `<span>` element inside a paragraph.
   `<span>Hello World</span> `
   Eg:
   The `<div>` element is often used as a container for other HTML elements.
   ```html
    <div style="background-color:black;color:white;padding:20px;">
    <h2>Heading</h2>
    <p>This is a sample text by using div element. So we can make the div element as a container .</p>
    </div>
  ```
  The `<span>` element is an inline container used to mark up a part of a text, or a part of a document.
  The `<span>` element has no required attributes, but style, class and id are common.
  ```html
     <p>I have a <span style="color:blue;font-weight:bold;">blue</span>
     pen and my brother has a  <span style="color:darkolivegreen;font-weight:bold;">dark green</span> pen.</p>
  ```
## 17_Div Element
  The `<div>` element is used as a container for other HTML elements.
  The `<div>` element is by default a block element, meaning that it takes all available width, and comes with line breaks before and after.
  The `<div>` element has no required attributes, but style, class and id are common.
Example
A `<div>` element with HTML elements:
```html
<div>
  <h2>London</h2>
  <p>London is the capital city of England.</p>
  <p>London has over 9 million inhabitants.</p>
</div>
```
Center align a `<div>` element
If you have a `<div>` element that is not 100% wide, and you want to center-align it, set the CSS margin property to auto.
Example
```html
<style>
div {
  width:300px;
  margin:auto;
}
</style>
```
Multiple `<div>` elements
You can have many `<div>` containers on the same page.
Example
```html
<div>
  <h2>London</h2>
  <p>London is the capital city of England.</p>
  <p>London has over 9 million inhabitants.</p>
</div>

<div>
  <h2>Oslo</h2>
  <p>Oslo is the capital city of Norway.</p>
  <p>Oslo has over 700,000 inhabitants.</p>
</div>

<div>
  <h2>Rome</h2>
  <p>Rome is the capital city of Italy.</p>
  <p>Rome has over 4 million inhabitants.</p>
</div>
```
There are different methods for aligning elements side by side, all include some CSS styling. We will look at the most common methods:
Float
The CSS float property was not originally meant to align `<div>` elements side-by-side, but has been used for this purpose for many years.
The CSS float property is used for positioning and formatting content and allows elements to be positioned horizontally, rather than vertically.
Example
```html
<style>
.mycontainer {
  width:100%;
  overflow:auto;
}
.mycontainer div {
  width:33%;
  float:left;
}
</style>
```
Inline-block
If you change the `<div>` element's display property from block to inline-block, the `<div>` elements will no longer add a line break before and after, and will be displayed side by side instead of on top of each other.
Example
How to use display: inline-block to align div elements side by side:
```html
<style>
div {
  width: 30%;
  display: inline-block;
}
</style>
```
Flex
The CSS Flexbox Layout Module was introduced to make it easier to design flexible responsive layout structure without using float or positioning.
To make the CSS flex method work, surround the `<div>` elements with another `<div>` element and give it the status as a flex container.
Example
How to use flex to align div elements side by side:
```html
<style>
.mycontainer {
  display: flex;
}
.mycontainer > div {
  width:33%;
}
</style>
```
Grid
The CSS Grid Layout Module offers a grid-based layout system, with rows and columns, making it easier to design web pages without having to use floats and positioning.
The CSS grid method requires that you surround the `<div>` elements with another `<div>` element and give the status as a grid container, and you must specify the width of each column.
Example
How to use grid to align `<div>` elements side by side:
```html
<style>
.grid-container {
  display: grid;
  grid-template-columns: 33% 33% 33%;
}
</style>
``` 
## 18_HTML ID's
 *  The id attribute is used to specify a unique id for an HTML element
 *  The value of the id attribute must be unique within the HTML document
 *  The id attribute is used by CSS and JavaScript to style/select a specific element
 *  The value of the id attribute is case sensitive
 *  The id attribute is also used to create HTML bookmarks
 *  JavaScript can access an element with a specific id with the getElementById() method
 *  In css id can be mentioned as `#` by mentioning the id name in the element
 **Note:**A class name can be used by multiple HTML elements, while an id name must only be used by one HTML element within the page
 **Eg**
 ```html
 <!DOCTYPE html>
<html>
<head>
<style>
#myHeader {
  background-color: lightblue;
  color: black;
  padding: 40px;
  text-align: center;
}
</style>
</head>
<body>

<h1 id="myHeader">My Header</h1>

</body>
</html>
```

**For Creation of Bookmark**

```html
First, create a bookmark with the id attribute:
<h2 id="I1">Introduction</h2>

Then, add a link to the bookmark , from within the same page:
Example
<a href="#I1">To learn from the begining go to introduction page!!</a>

Or, add a link to the bookmark , from another page:
<a href="html_demo.html#I1">Jump to Introduction</a>
```
## 19_IFrames
  HTML iframe is an inline frame that allows you to embed another document within the current HTML document. Whenever you want to display another webpage within the webpage, you can use an iframe. 
  ### Creating iframe (Inline Frame)
  `<iframe>` tag creates a rectangular region at a specified place within the HTML document 
  You can set the name height and width of an HTML iframe by using the height and width attributes of the `<iframe>` tag.
  `<iframe src="url" title="description"></iframe>`
  We can style the iframe by using external css.
  ### Multiple Iframes
  You can embed multiple documents (webpages) within a webpage. HTML allows you to use multiple `<iframe>` tags in an HTML document.
  **Note:** Use of multiple iframes may slow down your page loading speed.
## 20_Javascript in HTML
  JavaScript makes HTML pages more dynamic and interactive.
  Example
  My First JavaScript
  The HTML `<script>` Tag
  The HTML `<script>` tag is used to define a client-side script `(JavaScript)`.
  The `<script>` element either contains script statements, or it points to an external script file through the src attribute.
  Common uses for JavaScript are image manipulation, form validation, and dynamic changes of content.
  To select an HTML element, JavaScript most often uses the `document.getElementById()` method.
  This JavaScript example writes `"Hello JavaScript!"` into an HTML element with `id="demo"`:
  Example
```html
  <script>
  document.getElementById("demo").innerHTML = "Hello JavaScript!";
  </script>
  ```
  Here are some examples of what JavaScript can do:
  Example
  JavaScript can change content:
`document.getElementById("demo").innerHTML = "Hello JavaScript!";`
  JavaScript can change styles:
```html  
  <script>
  document.getElementById("demo").style.fontSize = "25px";
  document.getElementById("demo").style.color = "red";
  document.getElementById("demo").style.backgroundColor = "yellow";
  </script>
```
  Example
  JavaScript can change attributes:
  `document.getElementById("image").src = "picture.gif";`
  The HTML `<noscript>` Tag
  The HTML `<noscript>` tag defines an alternate content to be displayed to users that have disabled scripts in their browser or have a browser that doesn't support scripts:
  Example
```html
  <script>
  document.getElementById("demo").innerHTML = "Hello JavaScript!";
  </script>
<noscript>Sorry, your browser does not support JavaScript!</noscript> 
```
For learning the styling of javascript go to the javascript file
## 21_File Paths
  A file path describes the location of a file in a web site's folder structure.
  File Path Examples
```html
  Path	                      Description
  <img src="picture.jpg">    	The "picture.jpg" file is located in the same folder as the current page
  <img src="images/picture.jpg">The "picture.jpg" file is located in the images folder in the current folder
  <img src="/images/picture.jpg">The "picture.jpg" file is located in the images folder at the root of the current web
  <img src="../picture.jpg">  The "picture.jpg" file is located in the folder one level up from the current folder
```
  HTML File Paths
    A file path describes the location of a file in a web site's folder structure.
    File paths are used when linking to external files, like:
      Web pages
      Images
      Style sheets
      JavaScripts
Absolute File Paths
An absolute file path is the full URL to a file:
Example
`<img src="https://www.w3schools.com/images/picture.jpg" alt="Mountain">`
The `<img>` tag is explained in the chapter: HTML Images.
Relative File Paths
A relative file path points to a file relative to the current page.
In the following example, the file path points to a file in the images folder located at the root of the current website:
Example
`<img src="/images/picture.jpg" alt="Mountain">`
In the following example, the file path points to a file in the images folder located in the current folder:
Example
`<img src="images/picture.jpg" alt="Mountain">`
In the following example, the file path points to a file in the images folder located in the folder one level up from the current folder:
Example
`<img src="../images/picture.jpg" alt="Mountain">` 

## 22_Layouts
HTML has several semantic elements that define the different parts of a web page:
HTML5 Semantic Elements 	
    `<header>` - Defines a header for a document or a section
    `<nav>` - Defines a set of navigation links
    `<section>` - Defines a section in a document
    `<article>` - Defines independent, self-contained content
    `<aside>` - Defines content aside from the content (like a sidebar)
    `<footer>` - Defines a footer for a document or a section
    `<details>` - Defines additional details that the user can open and close on demand
    `<summary>` - Defines a heading for the `<details>` element
HTML Layout Techniques
There are four different techniques to create multicolumn layouts. Each technique has its pros and cons:
  * CSS frameworks
  * CSS float property
  * CSS flexbox
  * CSS grid
### CSS Frameworks
If you want to create your layout fast, you can use a CSS framework, like W3.CSS or Bootstrap.
### Float
The float property specifies how an element should float within its container.
It places an element on the left or right side of its container, allowing text and inline elements to wrap around it.
The float property can have one of the following values:
    left - The element floats to the left of its container
    right - The element floats to the right of its container
    none - Default. The element does not float and is displayed just where it occurs in the text
    inherit - The element inherits the float value of its parent
Tip: The float property is often used to wrap text around images!
### CSS Flexbox (Flexible Box Layout)
CSS Flexbox is short for the CSS Flexible Box Layout module.
Flexbox is a layout model for arranging items (horizontally or vertically) within a container, in a flexible and responsive way.
Flexbox makes it easy to design a flexible and responsive layout, without using float or positioning.
### Flexbox vs. Grid
CSS Flexbox is used for a one-dimensional layout, with rows OR columns.
CSS Grid is used for a two-dimensional layout, with rows AND columns.
CSS Flexbox Components
A flexbox always consists of:
    A Flex Container - The parent (container) element, where the display property is set to flex or inline-flex
    One or more Flex Items - The direct children of the flex container automatically becomes flex items
### CSS Grid Layout Module
The Grid Layout Module offers a grid-based layout system, with rows and columns.
The Grid Layout Module allows developers to easily create complex web layouts.
The Grid Layout Module makes it easy to design a responsive layout structure, without using float or positioning.
A grid always consists of:
    A Grid Container - The parent (container) element, where the display property is set to grid or inline-grid
    One or more Grid Items - The direct children of the grid container automatically becomes grid items
## 23_Responsive web design
  Responsive Web Design is about using HTML and CSS to automatically resize, hide, shrink, or enlarge, a website, to make it look good on all devices (desktops, tablets, and phones):
  ### Setting The Viewport
   To create a responsive website, add the following `<meta>` tag to all your web pages:
    Example
  `<meta name="viewport" content="width=device-width, initial-scale=1.0">`
    This will set the viewport of your page, which will give the browser instructions on how to control the page's dimensions and scaling.
  ### Responsive Images
  Responsive images are images that scale nicely to fit any browser size.
  Using the width Property
  If the CSS width property is set to 100%, the image will be responsive and scale up and down:
  Example
  `<img src="img_girl.jpg" style="width:100%;">`
Notice that in the example above, the image can be scaled up to be larger than its original size. A better solution, in many cases, will be to use the max-width property instead.
  Using the max-width Property
  If the max-width property is set to 100%, the image will scale down if it has to, but never scale up to be larger than its original size:
  Example
`<img src="img_girl.jpg" style="max-width:100%;height:auto;">`
  The HTML `<picture>` element allows you to define different images for different browser window sizes.
Example
```html
<picture>
  <source srcset="img_smallflower.jpg" media="(max-width: 600px)">
  <source srcset="img_flowers.jpg" media="(max-width: 1500px)">
  <source srcset="flowers.jpg">
  <img src="img_smallflower.jpg" alt="Flowers">
</picture>
```
Responsive Text Size
The text size can be set with a "vw" unit, which means the "viewport width".
Example
`<h1 style="font-size:10vw">Hello World</h1>`
Viewport is the browser window size. 1vw = 1% of viewport width. If the viewport is 50cm wide, 1vw is 0.5cm.
Media Queries
In addition to resize text and images, it is also common to use media queries in responsive web pages.
With media queries you can define completely different styles for different browser sizes.
Example: resize the browser window to see that the three div elements below will display horizontally on large screens and stack vertically on small screens:

## 24_Semantic Elements
  Semantic HTML tags are markup elements that clearly describe their meaning to both the browser and the developer.
  ### Common Semantic Tags
  `<header>`: Represents introductory content or a set of navigational links at the top of a page or section.
  `<nav>`: Defines a block of navigation links.
  `<main>`: Specifies the dominant, unique content of the body of a document.
  `<section>`: Groups related content that shares a thematic grouping or purpose.
  `<article>`: Holds self-contained, independent content like a blog post or news story.
  `<aside>`: Contains tangentially related content like sidebars or call-out boxes.
  `<footer>`: Houses footer information like copyright notices or author details. 
  ### Why Use Semantic Tags?
  Accessibility: Screen readers and assistive tools use these tags to help users navigate a page efficiently.
  SEO: Search engines better understand the structure and importance of your content.
  Maintainability: Code is cleaner and easier for other developers to read than a generic file full of `<div>` tags
```html
<body>

    <!-- Header: Page title and primary navigation -->
    <header>
        <h1>Sample Blog</h1>
        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#articles">Articles</a></li>
                <li><a href="#about">About</a></li>
            </ul>
        </nav>
    </header>

    <!-- Main: Unique, primary content of the document -->
    <main>
        
        <!-- Section: A distinct thematic grouping of content -->
        <section id="articles">
            <h2>Latest Tech Articles</h2>

            <!-- Article 1: Independent, self-contained post -->
            <article>
                <h3>Understanding Semantic HTML</h3>
                <p>Published on: <time datetime="2026-09-05">September 5, 2026</time></p>
                <p>Semantic tags give meaning to your web structure, making it highly accessible and SEO-friendly.</p>
                <a href="#read-more-1">Read full article...</a>
            </article>

            <!-- Article 2: Independent, self-contained post -->
            <article>
                <h3>The Future of CSS</h3>
                <p>Published on: <time datetime="2026-08-28">August 28, 2026</time></p>
                <p>Explore modern layout tools, container queries, and new functional selectors coming to CSS.</p>
                <a href="#read-more-2">Read full article...</a>
            </article>

        </section>

        <!-- Aside: Tangential or sidebar content -->
        <aside>
            <h3>About the Author</h3>
            <p>Alex is a frontend developer focused on building clean, fully accessible user experiences.</p>
            <h3>Newsletter Signup</h3>
            <form>
                <input type="email" placeholder="Enter your email" aria-label="Email address">
                <button type="submit">Subscribe</button>
            </form>
        </aside>

    </main>

    <!-- Footer: Copyright, terms, and contact links -->
    <footer>
        <p>&copy; 2026  All rights reserved.</p>
        <p><a href="#privacy">Privacy Policy</a> | <a href="#terms">Terms of Service</a></p>
    </footer>
</body>
```
## 25_Entities
  Reserved characters in HTML must be replaced with entities:
    < (less than) = &lt;
    > (greater than) = &gt;

  HTML Character Entities
  Some characters are reserved in HTML.
  If you use the less than `(<)` or greater than `(>)` signs in your HTML text, the browser might mix them with tags.
  Entity names or entity numbers can be used to display reserved HTML characters.
  Entity names look like this:
  `&entity_name;`
  Entity numbers look like this:
  `&#entity_number;`
  To display a less than sign (<) we must write: `&lt;` or `&#60;`

  Some Useful HTML Character Entities
```html
  Result 	Description 	         Name 	    Number 	
         non-breaking space 	   &nbsp; 	  &#160; 	
  < 	   less than               &lt; 	    &#60; 	
  > 	   greater than 	         &gt; 	    &#62; 	
  & 	   ampersand             	 &amp; 	    &#38; 	
  " 	   double quotation mark 	 &quot; 	  &#34; 	
  ' 	   single quotation mark 	 &apos; 	  &#39; 	
  ¢ 	   cent 	                 &cent; 	  &#162; 	
  £ 	   pound 	                 &pound;  	&#163; 	
  ¥ 	   yen                   	 &yen; 	    &#165; 	
  € 	   euro 	                 &euro; 	  &#8364; 	
  © 	   copyright 	             &copy; 	  &#169; 	
  ® 	   registered trademark 	 &reg;    	&#174; 	
  ™ 	   trademark 	             &trade;  	&#8482;
```
## 26_Encoding
URLs can only be sent over the Internet using the ASCII character-set. If a URL contains characters outside the ASCII set, the URL has to be converted.
encoding converts non-ASCII characters into a format that can be transmitted over the Internet.
encoding replaces non-ASCII characters with a "%" followed by hexadecimal digits.
URLs cannot contain spaces. URL encoding normally replaces a space with a plus (+) sign, or %20.
**Eg:Hello Günter is encoded as text=Hello+G%C3%BCnter**
## 27_URL Encoding
A URL is another word for a web address.
A URL can be composed of words ww.likeweb.com, or an Internet Protocol (IP) address (e.g. 192.68.20.50).
Most people enter the name when surfing, because names are easier to remember than numbers.
URL - Uniform Resource Locator
Web browsers request pages from web servers by using a URL.
A Uniform Resource Locator (URL) is used to address a document (or other data) on the web.
A web address like https://www.exampleweb.com/html/default.asp follows these syntax rules:
scheme://prefix.domain:port/path/filename

Explanation:
    scheme - defines the type of Internet service (most common is http or https)
    prefix - defines a domain prefix (default for http is www)
    domain - defines the Internet domain name (like w3schools.com)
    port - defines the port number at the host (default for http is 80)
    path - defines a path at the server (If omitted: the root directory of the site)
    filename - defines the name of a document or resource
Common URL Schemes

Scheme      	Short for 	                            Used for
http 	        HyperText Transfer Protocol 	          Common web pages. Not encrypted
https 	      Secure HyperText Transfer Protocol 	    Secure web pages. Encrypted
ftp 	        File Transfer Protocol 	                Downloading or uploading files
file 	  	                                            A file on your computer
## 28_Forms
An HTML form is used to collect user input. The user input is most often sent to a server for processing. 
  ### Form Elements
  `<form>` 	Defines an HTML form for user input
  `<input>` 	Defines an input control
  `<textarea>` 	Defines a multiline input control (text area)
  `<label>` 	Defines a label for an `<input>` element
  `<fieldset>` 	Groups related elements in a form
  `<legend>` 	Defines a caption for a `<fieldset>` element
  `<select>` 	Defines a drop-down list
  `<optgroup>` 	Defines a group of related options in a drop-down list
  `<option>` 	Defines an option in a drop-down list
  `<button>` 	Defines a clickable button
  `<datalist>` 	Specifies a list of pre-defined options for input controls
  `<output>` 	Defines the result of a calculation
  Here are some of the key attributes that can be used with the `<form>` element:
    action: Specifies the URL where the form data is sent upon submission.
    method: Defines the HTTP method used to send the data — either "get" or "post".
    target: Determines where to display the server’s response (e.g., "_blank", "_self", "_parent", "_top", or an iframe name).
    enctype: Specifies how form data is encoded when using method="post" (e.g., application/x-www-form-urlencoded, multipart/form-data, text/plain).
    autocomplete: Controls whether the browser should auto-fill form fields ("on" or "off").
    novalidate: A Boolean attribute that prevents the form from being validated before submission.
  Input Types in HTML Forms

Here are the commonly used input types in HTML Forms:
```html
  <input type="text">
  Defines a one-line text input field
  <input type="password">
  Defines a password field
  <input type="submit">
  Defines a submit button
  <input type="reset">
  Defines a reset button
  <input type="radio">
  Defines a radio button
  <input type="email">
  Validates that the input is a valid email address.
  <input type="number">
  Allows the user to enter a number. You can specify min, max, and step attributes for range.
  <input type="checkbox">
  Used for checkboxes where the user can select multiple options.
  <input type="date">
  Allows the user to select a date from a calendar.
  <input type="time">
  Allows the user to select a time.
  <input type="file">
  Allows the user to select a file to upload.
```
**Syntax**
```html
<form>
      <!--form elements-->
</form>
```
To view the sample code go to the forms file
## 29_Graphics
  There are two types in HTML Graphics
  * Canvas
  * SVG
  Canvas
    The HTML `<canvas>` element is used to draw graphics, on the fly, via JavaScript.
    The `<canvas>` element is only a container for graphics. You must use JavaScript to actually draw the graphics.
    Canvas has several methods for drawing paths, boxes, circles, text, and adding images.
    Canvas is supported by all major browsers.
    A canvas is a rectangular area on an HTML page. By default, a canvas has no border and no content.
The markup looks like this:
`<canvas id="myCanvas" width="200" height="100"></canvas>`
Always use the id attribute to link with the javascript code so that it can draws the shapes by using the js functions
Eg:
```html
<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.beginPath();
ctx.arc(95, 50, 40, 0, 2 * Math.PI);
ctx.stroke();
</script> 
```
  SVG
    SVG stands for Scalable Vector Graphics
    SVG is used to define vector-based graphics for the Web
    SVG defines graphics in XML format
    Each element and attribute in SVG files can be animated
    SVG is a W3C recommendation
    SVG integrates with other standards, such as CSS, DOM, XSL and JavaScript
  The `<svg>` Element
  The HTML `<svg>` element is a container for SVG graphics.
  SVG has several methods for drawing paths, rectangles, circles, polygons, text, and much more.
```html
  <svg width="100" height="100">
  <circle cx="50" cy="50" r="40" stroke="green" stroke-width="4" fill="yellow" />
</svg>
```
## 30_Media
  In html media can be added through the video,audio and you tube links
  The HTML `<video>` Element
  To show a video in HTML, use the `<video>` element:
  Example
```html
  <video width="320" height="240" controls>
    <source src="movie.mp4" type="video/mp4">
    <source src="movie.ogg" type="video/ogg">
  Your browser does not support the video tag.
  </video>
```
  How it Works
  The controls attribute adds video controls, like play, pause, and volume.
  It is a good idea to always include width and height attributes. If height and width are not set, the page might flicker while the video loads.
  The `<source>` element allows you to specify alternative video files which the browser may choose from. The browser will use the first recognized format.
  The text between the `<video>` and `</video>` tags will only be displayed in browsers that do not support the `<video>` element.
  HTML `<video>` Autoplay
  To start a video automatically, use the autoplay attribute:
  Example
```html
  <video width="320" height="240" autoplay>
    <source src="movie.mp4" type="video/mp4">
    <source src="movie.ogg" type="video/ogg">
  Your browser does not support the video tag.
  </video> 
```
  The HTML `<audio>` Element
  To play an audio file in HTML, use the `<audio>` element:
  Example
```html
  <audio controls>
    <source src="horse.ogg" type="audio/ogg">
    <source src="horse.mp3" type="audio/mpeg">
  Your browser does not support the audio element.
  </audio>
```
  HTML Audio - How It Works
  The controls attribute adds audio controls, like play, pause, and volume.
  The `<source>` element allows you to specify alternative audio files which the browser may choose from. The browser will use the first recognized format.
  The text between the `<audio>` and `</audio>` tags will only be displayed in browsers that do not support the `<audio>` element.
  HTML `<audio>` Autoplay
  To start an audio file automatically, use the autoplay attribute:
  Example
```html
  <audio controls autoplay>
    <source src="horse.ogg" type="audio/ogg">
    <source src="horse.mp3" type="audio/mpeg">
  Your browser does not support the audio element.
  </audio>
```
  Add muted after autoplay to let your audio file start playing automatically (but muted):
  Example
```html
  <audio controls autoplay muted>
    <source src="horse.ogg" type="audio/ogg">
    <source src="horse.mp3" type="audio/mpeg">
  Your browser does not support the audio element.
  </audio> 
```
  PLug ins
  Plug-ins were designed to be used for many different purposes:
    To run Java applets
    To run Microsoft ActiveX controls
    To display Flash movies
    To display maps
    To scan for viruses
    To verify a bank id
  But now most of the plugins were not supported by the browsers
  The `<object>` Element
  The `<object>` element is supported by all browsers.
  The `<object>` element defines an embedded object within an HTML document.
  It was designed to embed plug-ins (like Java applets, PDF readers, and Flash Players) in web pages, but can also be used to include HTML in HTML
  Example
  `<object width="100%" height="500px" data="snippet.html"></object>`
  Or images if you like:
  Example
  `<object data="audi.jpeg"></object>`
  The `<embed>` Element
  The `<embed>` element is supported in all major browsers.
  The `<embed>` element also defines an embedded object within an HTML document.
  Web browsers have supported the `<embed>` element for a long time. However, it has not been a part of the HTML specification before HTML5.
  Example
  `<embed src="audi.jpeg">`
  Note that the `<embed>` element does not have a closing tag. It can not contain alternative text.
  The `<embed>` element can also be used to include HTML in HTML:
  Example
  `<embed width="100%" height="500px" src="snippet.html">`
  The easiest way to play videos in HTML, is to use YouTube.
Converting videos to different formats can be difficult and time-consuming.
An easier solution is to let YouTube play the videos in your web page.
Playing a YouTube Video in HTML
To play your video on a web page, do the following:
    Upload the video to YouTube
    Take a note of the video id
    Define an `<iframe>` element in your web page
    Let the src attribute point to the video URL
    Use the width and height attributes to specify the dimension of the player
    Add any other parameters to the URL (see below)
Example
```html
<iframe width="420" height="315"
src="https://www.youtube.com/embed/tgbNymZ7vqY">
</iframe>
```
YouTube Autoplay + Mute
You can let your video start playing automatically when a user visits the page, by adding autoplay=1 to the YouTube URL. 
Add mute=1 after autoplay=1 to let your video start playing automatically (but muted).
YouTube - Autoplay + Muted
```html
<iframe width="420" height="315"
src="https://www.youtube.com/embed/tgbNymZ7vqY?autoplay=1&mute=1">
</iframe>
```
A comma separated list of videos to play (in addition to the original URL).
YouTube Loop
Add playlist=videoID and loop=1 to let your video loop forever.
loop=0 (default) - The video will play only once.
loop=1 - The video will loop (forever).
YouTube - Loop forever
```html
<iframe width="420" height="315"
src="https://www.youtube.com/embed/tgbNymZ7vqY?playlist=tgbNymZ7vqY&loop=1">
</iframe>
```
YouTube Controls
Add controls=0 to NOT display controls in the video player.
controls=0 - Player controls does not display.
controls=1 (default) - Player controls is displayed.
YouTube - Controls
```html
<iframe width="420" height="315"
src="https://www.youtube.com/embed/tgbNymZ7vqY?controls=0">
</iframe>  
```
```

 

 

 
