HTML: 

Elements of HTML: 

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

Eg: <a href="https://www.google.com">Visit Google</a> 

href attribute: 
  <a> tag defines a hyperlink. Then href specifies the URL of the page that goes 

src attribute: 
  <img> tag is used for embed an image in an HTML page. src represents the path to the image to be displayed. 
<img src="img_sample.jpeg"> 

  

url can be displayed in two ways: 
Absolute URL:  Links an external image that is hosted on another website 
eg: 
src=”https://static.wixstatic.com/media/2b9330_dd668a2e1d664129a64eba0689ffd142~mv2_d_1920_1386_s_2.jpg/v1/fill/w_560,h_374,al_c,q_80,usm_0.66_1.00_0.01,enc_avif,quality_auto/africa-animal-big-cat-88234.jpg” 

Note: by using the external links might be under copyright. If you do not get permission to use it, you may be in violation of copyright laws. In addition, you cannot control external images; it can suddenly be removed or changed. 

Relative URL: Links to an image that is hosted in within the website 
Eg: src=”image_sample.png” 

Note : always best to use relative URLs.This will  not affect any webpages. 

Width and height attributes: 
Image tag also contain the width and the height tags that can be used for adjusting the height and width of the image.  
Eg:<img src=”img_sample.jpg” height=”200px” width=”300px”> 

Alt attributes: 
Alt attributes can be used in the situation of whether the image is not displayed on the webpage 

Eg: when the image is in the absolute url and there’s no internet connection means then the altenative text content can be displayed. 

Style attribute: 
The style attribute is used to add styles to an element, such as color, font, size, and more. 

Eg:It can be used for the inline css. 

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
Eg: Superscript text can be used for footnotes, like WWW[1]

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

 

 

 

 