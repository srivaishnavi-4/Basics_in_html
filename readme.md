<<<<<<< HEAD
```
#HTML:#
##Working of HTML:## 
An external web server stores your HTML files and sends them to a user's web browser over the internet when requested
  On an external server:
  The Request: You type a website address into your browser. Your browser sends an HTTP request across the internet to the external server's IP address.
  The Lookup: The server receives the request, looks in its storage folders for the requested HTML file (such as index.html), and prepares a reply.
  The Response: The server sends the raw HTML text back to your browser with a success status code (like 200 OK).
  The Rendering: Your browser reads the incoming HTML code and turns it into the visual webpage you see on your screen.
  Loading Extra Files: If your HTML links to other files like CSS stylesheets, JavaScript, or images, your browser sends separate, follow-up requests to the server to grab those pieces.
`
   http://   localhost   :3000   /assets/styles.css   ?theme=dark
  ──┬──    ────┬────   ──┬──   ────────┬─────────   ─────┬─────
    │          │         │             │                 └── Query Parameters
    │          │         │             │                     (Data sent to server)
    │          │         │             └── Pathname 
    │          │         │                 (Target file system structure)
    │          │         └── Port Number 
    │          │             (Directs traffic to your specific dev tool)
    │          └── Hostname 
    │              (Mapped internally by your computer to IP 127.0.0.1)
    └── Protocol/Scheme 
        (Usually unencrypted HTTP during development)
`
##HTML Document Format:## 
  Document type Declaration: 
  This statement tells the web browser what versin of HTML the document is written in.It helps the browser interpret and display the code correctly. 
=======
```HTML: 
>>>>>>> 427f29b3ffc958e22969fe4d0346c3376e485855

    ` <!DOCTYPE html> `

<<<<<<< HEAD
  HTML Tag: 
  It is the starting point or the main container of the webpage.It is like the root or base of a tree which other elements are branch out.All the text,images and links is nested with this HTML Tag. 

     ` <html> `

  Head: 
  The head section is like a store room for important details about the webpage,such as its title,design,instructions and extra features.It contains the background information that helps the webpage function correctly and look good. 
      `<head><!--Other meta information--></head> `
  Body:
  the body section of a webpage is where you find all the main content like text,images,headings,and lists.
##1_Elements of HTML: ##
`
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
`
  Essential HTML Elements: 
  Elements are the building blocks of HTML. These are the tags that can we used everyday. 
  Basic
 ` <h1> to <h6> 	Defines HTML headings
  <p> 	Defines a paragraph
  <br> 	Inserts a single line break
  <hr> 	Defines a thematic change in the content
  <!--...--> 	Defines a comment
`
  Formatting
  `<b> - Bold text
  <strong> - Important text
  <i> - Italic text
  <em> - Emphasized text
  <mark> - Marked text
  <small> - Smaller text
  <del> - Deleted text
  <ins> - Inserted text
  <sub> - Subscript text
  <sup> - Superscript text
  `
  Forms
  `<form> 	Defines an HTML form for user input
  <input> 	Defines an input control
  <textarea> 	Defines a multiline input control (text area)
  <button> 	Defines a clickable button
  <select> 	Defines a drop-down list
  <optgroup> 	Defines a group of related options in a drop-down list
  <option> 	Defines an option in a drop-down list
  <label> 	Defines a label for an <input> element
  <fieldset> 	Groups related elements in a form
  <legend> 	Defines a caption for a <fieldset> element
  <datalist> 	Specifies a list of pre-defined options for input controls
  <output> 	Defines the result of a calculation`
=======
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

Essential HTML Elements: 

Elements are the building blocks of HTML. These are the tags that can we used everyday. 

Attributes: 

All HTML elements can have attributes 

Attributes provide additional information about elements 

Attributes are always specified in the start tag 

Attributes usually come in name/value pairs like: name="value" 
>>>>>>> 427f29b3ffc958e22969fe4d0346c3376e485855

  Links
  `<a> 	Defines a hyperlink
  <link> 	Defines the relationship between a document and an external resource (most used to link to style sheets)
  <nav> 	Defines navigation links`

<<<<<<< HEAD
##2_Attributes:## 
  All HTML elements can have attributes 
  Attributes provide additional information about elements 
  Attributes are always specified in the start tag 
  Attributes usually come in name/value pairs like: name="value" 

  `Eg: <a href="https://www.google.com">Visit Google</a>` 
=======
href attribute: 

  <a> tag defines a hyperlink. Then href specifies the URL of the page that goes 

src attribute: 

  <img> tag is used for embed an image in an HTML page. src represents the path to the image to be displayed. 

<img src="img_sample.jpeg"> 
>>>>>>> 427f29b3ffc958e22969fe4d0346c3376e485855

  href attribute: 
    <a> tag defines a hyperlink. Then href specifies the URL of the page that goes 

  src attribute: 
    <img> tag is used for embed an image in an HTML page. src represents the path to the image to be displayed. 
  `<img src="img_sample.jpeg"> `

  url can be displayed in two ways: 
  Absolute URL:  Links an external image that is hosted on another website 
  eg: 
  `src=”https://static.wixstatic.com/media/2b9330_dd668a2e1d664129a64eba0689ffd142~mv2_d_1920_1386_s_2.jpg/v1/fill/w_560,h_374,al_c,q_80,usm_0.66_1.00_0.01,enc_avif,quality_auto/africa-animal-big-cat-88234.jpg” 
  `
  Note: by using the external links might be under copyright. If you do not get permission to use it, you may be in violation of copyright laws. In addition, you cannot control external images; it can suddenly be removed or changed. 

  Relative URL: Links to an image that is hosted in within the website 
  `Eg: src=”image_sample.png” `

  Note : always best to use relative URLs.This will  not affect any webpages. 

  Width and height attributes: 
  Image tag also contain the width and the height tags that can be used for adjusting the height and width of the image.  
  `Eg:<img src=”img_sample.jpg” height=”200px” width=”300px”>` 

  Alt attributes: 
    Alt attributes can be used in the situation of whether the image is not displayed on the webpage 
    Eg: when the image is in the absolute url and there’s no internet connection means then the altenative text content can be displayed. 
    `<img src=”img_sample.jpg” alt="sample image" height=”200px” width=”300px”>` 


  Style attribute: 
  The style attribute is used to add styles to an element, such as color, font, size, and more. 
  Eg:It can be used for the inline css. 
  `<p style="color:red;">This is a paragraph</p>


  Lang attribute: 
  Lang attribute mentions the language of the webpage which is inside the html tag. 
  `<!DOCTYPE html>
  <html lang="en">`

  The title Attribute 
  The title attribute defines some extra information about an element. 
  The value of the title attribute will be displayed as a tooltip when you mouse over the element
  `<p title="This is a tooltip">This is a pararaph</p>`

##3_Head tags <h1> to <h6>:## 
  HTML provides the 6 levels of headings <h1> is the most important <h6> is the least important. 
  Search engines use the headings to index the structure and content of your web pages. 
  Users often skim a page by its headings. It is important to use headings to show the document structure. 
  <h1> headings should be used for main headings, followed by <h2> headings, then the less important <h3>, and so on. 

  For example: 
`  <h1> - Page title 
  <h2> - Section titles 
  <h3> - Sub-sections `
  Each heading has a default  size details. We can specify the size by using the style attribute. 

##4_Paragraph tags: ##
  A<p> tag starts on a new line and browsers automatically add some white space before and after the paragraph. 

  Note: 
  Eg:  `
  <p> This is a paragraph.This one is the line</p> 
  <p>This is another paragraph</p>.This works 
  <p>This is one paragraph 
  This is another</p>.This doesn’t works because the <p> tag automatically remove the whitespace from the browser. This is the poem problem. 
  To overcome this, we can use the <pre> tag 
`
  Pre Tag: 
  The HTML <pre> element defines preformatted text. 
  The text inside a <pre> element is displayed in a fixed-width font (usually Courier), and it preserves both spaces and line breaks 

##5_Styles: ##
  Style attribute is used to add styles to an element such as color,font size,and more; 
  Syntax: 
  <tagname style=”property:value;”> 
  Within style attribute we can build the inbuilt css features. 

  Background color: 
  It defines the background-color of a n HTML element. 

  Text color: 
  Color property defines the text color of an HTML element. 

  Fonts: 
  Font-family property defines the font to be used for an HTML element. 

  Text Size: 
  CSS font-size defines the text size for a HTML element. 

  Text Alignment: 
  CSS text-align defines the horizontal text alignment for an HTML element. 

##6_Quotation and Citation Elements##

  `  <blockquote>,<q>,<abbr>,<address>,<cite>,<bdo> `
  <blockquote>defines a section that is quoted from another source;
  usually it can be rendered by italic.
  
  `<blockquote cite="https://localhost:300">Here's a sample blockquote paragraph which can be intended
             .It can be quoted from another source</blockquote><!--blockquoted text-->`

<<<<<<< HEAD
  <q> short quoted text
    it is used for short quotation
    Browsers usually insert the quotation marks for the short quotes.
    `<q>This is a short quoted text</q><!--shortquoted text-->`
=======
url can be displayed in two ways: 

Absolute URL:  Links an external image that is hosted on another website 

eg: 

src=”https://static.wixstatic.com/media/2b9330_dd668a2e1d664129a64eba0689ffd142~mv2_d_1920_1386_s_2.jpg/v1/fill/w_560,h_374,al_c,q_80,usm_0.66_1.00_0.01,enc_avif,quality_auto/africa-animal-big-cat-88234.jpg” 
>>>>>>> 427f29b3ffc958e22969fe4d0346c3376e485855

  <abbr>abbrevation quotes
    it is used for the full form of the words.
    `<p>The <abbr title="World Health Organization">WHO</abbr> released a new artile about the recent war</p>`
  
  <address> it is used for contact information  like address,mobile number and email
   `<address>Written and mentioned by<br>
            The author,and their team<br>
            The book name,<br>
            location address</address>`
  
  <cite> mentions the title of a creative work(book,poem,song,movie,painting,sculpture etc) not the person.
   it usually renders in italic.
    ` <p>The <cite>book</cite> which was written by the author was published successfully</p> `

<<<<<<< HEAD
  <bdo> Bidirectional Override
    Override the current text direction.
    `<bdo dir="rtl">This is a reversed text</bdo>`
=======
Relative URL: Links to an image that is hosted in within the website 

Eg: src=”image_sample.png” 
>>>>>>> 427f29b3ffc958e22969fe4d0346c3376e485855

##7_Text Formatting: ##
  Formatting is used to display special types of text 
 ` <b> - Bold text 
  <strong> - Important text 
  <i> - Italic text 
  <em> - Emphasized text 
  <mark> - Marked text 
  <small> - Smaller text 
  <del> - Deleted text 
  <ins> - Inserted text 
  <sub> - Subscript text 
  <sup> - Superscript text 
`
  The difference between the  <b> and <strong>: 
  <b> defines the text without any importance . 
  <strong> it shows with strong importance .The content also displayed in bold. 
  Where we use <b> tag: 
  For  making the bold text in headings. 
  Eg: Topic1 

<<<<<<< HEAD
  Where we use <strong> tag: 
  For mentioning the importantance of word in a text. 
  Eg: This conversation is highly confidential. 

  Difference between the <i> and <em> tgs: 
  The HTML <i> element defines a part of text in an alternate voice or mood. The content inside is typically displayed in italic. 
  Tip: The <i> tag is often used to indicate a technical term, a phrase from another language, a thought, a ship name, etc. 
  Eg:     <i>This text is italic</i>  
=======
Width and height attributes: 

Image tag also contain the width and the height tags that can be used for adjusting the height and width of the image.  

Eg:<img src=”img_sample.jpg” height=”200px” width=”300px”> 

Alt attributes: 

Alt attributes can be used in the situation of whether the image is not displayed on the webpage 
>>>>>>> 427f29b3ffc958e22969fe4d0346c3376e485855

  The HTML <em> element defines emphasized text. The content inside is typically displayed in italic. 
  Tip: A screen reader will pronounce the words in <em> with an emphasis, using verbal stress. 
  Eg:  <em>This text is emphasized</em> 
`
  <small>- makes the text smaller 
  <mark > makes the text marked and highlighted 
  <del> the selected text be individually deleted 
  <ins> defines a text that has been inserted into the document 
  <sub> element defines subscript text. Subscript text appears half a character below the normal line, and is sometimes rendered in a smaller font.  
  Eg: Subscript text can be used for chemical formulas, like H2O 
  <sup> element defines superscript text. Superscript text appears half a character above the normal line, and is sometimes rendered in a smaller font.  
  Eg: Superscript text can be used for footnotes, like WWW[1]
`
##8_HTML Comment Tag:## 
  We can add comments to your HTML source by using the following syntax: 
  `<!-- Write your comments here --> ` 

<<<<<<< HEAD
  Note1: that there is an exclamation point (!) in the start tag, but not in the end tag. 
  Note2: Comments are not displayed by the browser, but they can help document your HTML source code. 
=======
Style attribute: 

The style attribute is used to add styles to an element, such as color, font, size, and more. 
>>>>>>> 427f29b3ffc958e22969fe4d0346c3376e485855

##10_HTML CSS Styles:## 
  Css can be used to format the layout of a webpage. 
  With CSS, you can control the color, font, the size of text, the spacing between elements, how elements are positioned and laid out, what background images or background colors are to be used, different displays for different devices and screen sizes, and all.. 
  Using CSS 
  CSS can be added to HTML documents in 3 ways: 

<<<<<<< HEAD
  Inline - by using the style attribute inside HTML elements 
  Internal - by using a <style> element in the <head> section 
  External - by using a <link> element to link to an external CSS file 

  The most common way to add CSS, is to keep the styles in external CSS files. However, in this tutorial we will use inline and internal styles, because this is easier to demonstrate, and easier for you to try it yourself. 

  Inline CSS 
  An inline CSS is used to apply a unique style to a single HTML element. 
  It uses the style attribute of an HTML element. 
  Eg: it sets the text color of the <h1> element to blue, and the text color of the <p> element to red. 
`
  <h1 style="color:blue;">A Blue Heading</h1> 
  <p style="color:red;">A red paragraph.</p> 
`
  Internal CSS 
  An internal CSS is used to define a style for a single HTML page.It is defined in the <head> section of an HTML page, within a <style> element. 
  Eg: we can set the text color of ALL the <h1> elements (on that page) to blue, and the text color of ALL the <p> elements to red. In addition, the page will be displayed with a "powderblue" background color. 
 `
  <style> 
  body {background-color: powderblue;} 
  h1   {color: blue;} 
  p    {color: red;} 
  </style> 
  <h1>This is a heading</h1> 
  <p>This is a paragraph.</p>
`
  External CSS 
  An external style sheet is used to define the style for many HTML pages. 
  To use an external style sheet, add a link to it in the <head> section of each HTML page: 
  Eg: 
 `
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
`
  CSS Color,Font-size,Font –family: 
      color property defines the text color to be used. 
      font-family property defines the font to be used. 
      font-size property defines the text size to be used. 
  For implementation refer the styles topic 

  CSS Border 
    The CSS border property defines a border around an HTML element. 
    Note: we can define a border for nearly all HTML elements. 
    `Eg:   p {border: 2px solid powderblue;} `

  CSS Padding 
    The CSS padding property defines a padding (space) between the text and the border. 
    Eg: 
  `
  p { 
    border: 2px solid powderblue; 
    padding: 30px; 
  }  
`
  CSS Margin 
    The CSS margin property defines a margin (space) outside the border. 
    Eg: 
  `
  p { 
    border: 2px solid powderblue; 
    margin: 50px; 
  }  
`
  Relation between Margin and Padding and Border 
  +-----------------------------------------------------------+
  |                        MARGIN                             |
  |    (Creates space between this element and others)        |
  |  +-----------------------------------------------------+  |
  |  |                     BORDER                          |  |
  |  |     (The visible outline around the element)        |  |
  |  |  +-----------------------------------------------+  |  |
  |  |  |                  PADDING                      |  |  |
  |  |  |    (Creates space between border and content) |  |  |
  |  |  |  +-----------------------------------------+  |  |  |
  |  |  |  |               CONTENT                   |  |  |  |
  |  |  |  |         (Text, images, etc.)            |  |  |  |
  |  |  |  +-----------------------------------------+  |  |  |
  |  |  +-----------------------------------------------+  |  |
  |  +-----------------------------------------------------+  |
  +-----------------------------------------------------------+

  Link to External CSS 
  External style sheets can be refered with a full URL or with a path relative to the current web page.

##11_HTML LINKS ##
  Text Links:
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

`   <a href="https://www.google.com" target="_self">Click for google!!!</a><br><!--_self-->
    <a href="https://www.stackoverflow.com" target="_parent">Click for stack overflow!!</a><br><!--_parent-->
    <a href="https://www.google.com" target="_top">Click for google!!!</a>  <br><!--_top-->
    <a href="https://www.google.com" target="_blank">Click for google!!!</a>  <br><!--_blank-->`
  Security with rel Attribute
  When you open links in new tabs using target="_blank", you need to add a security measure. Without it, the new page could potentially access your original page and cause problems.
  The rel="noopener noreferrer" attribute prevents the new page from accessing your original page. Always include this when using target="_blank"
    noopener: Prevents the new page from accessing the window object of your original page. This stops potential security exploits.
    noreferrer: Prevents sending referrer information to the new page. This adds privacy by not telling the destination site where the visitor came from.
    `<a href="https://www.google.com" target="_blank" rel="noopener noreferrer">Click for google safely!!!</a>  <br><!--_blank with noopener and norefferer-->`
  Use Image as a link:
    To use an image as a link, just put the <img> tag inside the <a> tag:
    `      <a href="https://medium.com"><img src="\gif_image.gif" alt="mushroom image"/></a>`

  Here are some example codes that explain the usage of image links in HTML:
    Create Hyperlink for an Image
    Image Link with Tooltip
    Mouse-Sensitive Images
        Server-Side Image Maps
        Client-Side Image Maps
    Image link with tooltip:
      You can also define a tooltip for an image link; when someone moves the mouse over the linked image, it will display a tooltip. To set the tooltip, you can set the title attribute of the <a> tag.
      `<a href="https://medium.com" title="go to medium"><img src="\gif_image.gif" alt="mushroom image"/></a><!--image with tooltip-->`
    Mouse sensitive images:
      HTML provides a feature that embed the different types of links in the single image then we can add the different links based on the co ordinates.such mouse sesitive images are known as image maps.
      In image maps there are  two types:
        Server-side image maps: This is enabled by the ismap attribute of the <img> tag and requires access to a server and related image-map processing applications.
        Client-side image maps: This is created with the usemap attribute of the <img> tag, along with corresponding <map> and <area> tags.
      In HTML, ismap and usemap are attributes used to create image maps, which turn an image into a set of multiple clickable links or regions. The core difference comes down to where the processing happens: ismap works on the server side, while usemap works on the client side (the browser).

      `<br><p>with usemap</p>
      <!--Use map-->
      <br><img src="\gif_image.gif" usemap="#shape-map" alt="Interactive Shapes">
      <map name="shape-map">
      <!-- Clickable rectangle area -->
      <area shape="rect" coords="34,44,270,350" href="https://www.google.com" alt="Rectangle Page">
      <!-- Clickable circle area -->
      <area shape="circle" coords="450,200,60" href="https://www.medium.com" alt="Circle Page">
      </map>
     <br> <p>with ismap</p>
      <br><a href="https://medium.com"><img src="\gif_image.gif" ismap alt="mushroom image"/></a><br><!--image with ismap-->
      `

    HTML Email Links:
      HTML email links allow users to click on a link and automatically open their default email client with a new message composed to the specified email address.
      This is done using the mailto: protocol in the href attribute of an <a> (anchor) tag.
      we can also predefine the subject and body of the email using the mailto: protocol. 
      This is done by appending ?subject= and &body= to the email address. Spaces and special characters in the subject and body should be URL-encoded. 
      For example, spaces are encoded as %20.

        `  <a href="mailto:example@example.com?subject=Hello%20there&body=This%20is%20a%20predefined%20email%20body."> 
      Click here to Send Mail</a>`

      Cons
          Adding an HTML email link to your webpage can expose your email address to spam. Automated programs, known as email harvesters, can scan web pages for email addresses and add them to spam lists.
           This can result in a significant increase in unwanted emails.

##12_HTML Image tag:## 
  The HTML <img> tag is used to embed an image in a web page. 
  Images are not technically inserted into a web page; images are linked to web pages. The <img> tag creates a holding space for the referenced image. 
  The <img> tag is empty, it contains attributes only, and does not have a closing tag. 
  The <img> tag has two required attributes: 
  src - Specifies the path to the image 
  alt - Specifies an alternate text for the image 
  Syntax : 
    `<img src="url" alt="alternatetext">` 
  The attributes like src,alt,height and width are mentioned on the attributes topic. 
  We can also add the gif formated images on the web by using web server. 

  Images in Another Folder: 
  If you have your images in a sub-folder, you must include the folder name in the src attribute: 
  Example 

     `<img src="/images/html5.gif" alt="HTML5 Icon" style="width:128px;height:128px;">` 

 ```
=======
Lang attribute: 

Lang attribute mentions the language of the webpage which is inside the html tag. 

The title Attribute 

The title attribute defines some extra information about an element. 

The value of the title attribute will be displayed as a tooltip when you mouse over the element: 

Head tags <h1> to <h6>: 

HTML provides the 6 levels of headings <h1> is the most important <h6> is the least important. 

Search engines use the headings to index the structure and content of your web pages. 

Users often skim a page by its headings. It is important to use headings to show the document structure. 

<h1> headings should be used for main headings, followed by <h2> headings, then the less important <h3>, and so on. 

For example: 

<h1> - Page title 

<h2> - Section titles 

<h3> - Sub-sections 

Each heading has a default  size details. We can specify the size by using the style attribute. 

Paragraph tags: 

A<p> tag starts on a new line and browsers automatically add some white space before and after the paragraph. 

Note: 

Eg:  

 <p> This is a paragraph.This one is the line</p> 

<p>This is another paragraph</p>.This works 

<p>This is one paragraph 

This is another</p>.This doesn’t works because the <p> tag automatically remove the whitespace from the browser. This is the poem problem. 

To overcome this, we can use the <pre> tag 

Pre Tag: 

The HTML <pre> element defines preformatted text. 

The text inside a <pre> element is displayed in a fixed-width font (usually Courier), and it preserves both spaces and line breaks 

Styles: 

Style attribute is used to add styles to an element such as color,font size,and more; 

Syntax: 

<tagname style=”property:value;”> 

Within style attribute we can build the inbuilt css features. 

Background color: 

It defines the background-color of a n HTML element. 

Text color: 

Color property defines the text color of an HTML element. 

Fonts: 

Font-family property defines the font to be used for an HTML element. 

Text Size: 

CSS font-size defines the text size for a HTML element. 

Text Alignment: 

CSS text-align defines the horizontal text alignment for an HTML element. 

Text Formatting: 

Formatting is used to display special types of text 

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

The difference between the  <b> and <strong>: 

<b> defines the text without any importance . 

<strong> it shows with strong importance .The content also displayed in bold. 

Where we use <b> tag: 

 For  making the bold text in headings. 

Eg: Topic1 

Where we use <strong> tag: 

For mentioning the importantance of word in a text. 

Eg: This conversation is highly confidential. 

Difference between the <i> and <em> tgs: 

The HTML <i> element defines a part of text in an alternate voice or mood. The content inside is typically displayed in italic. 

Tip: The <i> tag is often used to indicate a technical term, a phrase from another language, a thought, a ship name, etc. 

Eg:     <i>This text is italic</i>  

The HTML <em> element defines emphasized text. The content inside is typically displayed in italic. 

Tip: A screen reader will pronounce the words in <em> with an emphasis, using verbal stress. 

Eg:  <em>This text is emphasized</em> 

<small>- makes the text smaller 

<mark > makes the text marked and highlighted 

<del> the selected text be individually deleted 

<ins> defines a text that has been inserted into the document 

<sub> element defines subscript text. Subscript text appears half a character below the normal line, and is sometimes rendered in a smaller font.  

Eg: Subscript text can be used for chemical formulas, like H2O 

<sup> element defines superscript text. Superscript text appears half a character above the normal line, and is sometimes rendered in a smaller font.  

Eg: Superscript text can be used for footnotes, like WWW[1]: 

 

HTML Comment Tag: 

We can add comments to your HTML source by using the following syntax: 

<!-- Write your comments here -->  

Note1: that there is an exclamation point (!) in the start tag, but not in the end tag. 

Note2: Comments are not displayed by the browser, but they can help document your HTML source code. 

HTML CSS Styles: 

Css can be used to format the layout of a webpage. 

With CSS, you can control the color, font, the size of text, the spacing between elements, how elements are positioned and laid out, what background images or background colors are to be used, different displays for different devices and screen sizes, and all.. 

Using CSS 

CSS can be added to HTML documents in 3 ways: 

Inline - by using the style attribute inside HTML elements 

Internal - by using a <style> element in the <head> section 

External - by using a <link> element to link to an external CSS file 

The most common way to add CSS, is to keep the styles in external CSS files. However, in this tutorial we will use inline and internal styles, because this is easier to demonstrate, and easier for you to try it yourself. 

Inline CSS 

An inline CSS is used to apply a unique style to a single HTML element. 

It uses the style attribute of an HTML element. 

Eg: it sets the text color of the <h1> element to blue, and the text color of the <p> element to red. 

<h1 style="color:blue;">A Blue Heading</h1> 
<p style="color:red;">A red paragraph.</p> 

Internal CSS 

An internal CSS is used to define a style for a single HTML page.It is defined in the <head> section of an HTML page, within a <style> element. 

Eg: we can set the text color of ALL the <h1> elements (on that page) to blue, and the text color of ALL the <p> elements to red. In addition, the page will be displayed with a "powderblue" background color. 
<style> 
 body {background-color: powderblue;} 
h1   {color: blue;} 
p    {color: red;} 
 </style> 
<h1>This is a heading</h1> 
<p>This is a paragraph.</p> 
External CSS 

An external style sheet is used to define the style for many HTML pages. 

To use an external style sheet, add a link to it in the <head> section of each HTML page: 

Eg: 

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

CSS Color,Font-size,Font –family: 

color property defines the text color to be used. 

font-family property defines the font to be used. 

font-size property defines the text size to be used. 

For implementation refer the styles topic 

CSS Border 

The CSS border property defines a border around an HTML element. 

Note: we can define a border for nearly all HTML elements. 

Eg:   p {border: 2px solid powderblue;} 

CSS Padding 

The CSS padding property defines a padding (space) between the text and the border. 

Eg: 

p { 
  border: 2px solid powderblue; 
  padding: 30px; 
}  

CSS Margin 

The CSS margin property defines a margin (space) outside the border. 

Eg: 

p { 
  border: 2px solid powderblue; 
  margin: 50px; 
 }  

Relation between Margin and Padding and Border 

 

Link to External CSS 

External style sheets can be refered with a full URL or with a path relative to the current web page. 

HTML Image tag: 

The HTML <img> tag is used to embed an image in a web page. 

Images are not technically inserted into a web page; images are linked to web pages. The <img> tag creates a holding space for the referenced image. 

The <img> tag is empty, it contains attributes only, and does not have a closing tag. 

The <img> tag has two required attributes: 

src - Specifies the path to the image 

alt - Specifies an alternate text for the image 

Syntax : 

<img src="url" alt="alternatetext"> 

The attributes like src,alt,height and width are mentioned on the attributes topic. 

We can also add the gif formated images on the web by using web server. 

Images in Another Folder: 

If you have your images in a sub-folder, you must include the folder name in the src attribute: 

Example 

<img src="/images/html5.gif" alt="HTML5 Icon" style="width:128px;height:128px;"> 

 
>>>>>>> 427f29b3ffc958e22969fe4d0346c3376e485855

 ```

 

 
