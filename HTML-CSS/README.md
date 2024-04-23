# HTML-CSS
## Week 1: Introduction to HTML (Unit 1)

-HTML is a language that is able to declare instructions. It is a resiliant, robust and can be functional even with broken code.
-CSS is solely responsible for styling and animations of a web page. It is fragile and powerful. Once it detects broken code, the browser skips the code.
-Javascript is a delicate and sensitive language that does not run if it comes accross issues. It functions as an enhancer to websites.


## Week 1: HTML Text Formating (Unit 2)
-HTML uses tags to mark different elements which consist of an opening and closing tags.
-The tags form elements and can be nested inside elements.
-The structure of HTML is a Document Object Model (DOM) which connects web pages to scripts represented in a document.
-HTMl elements can be nested within one another, this is how an entire HTML document is structured.

## Week 1: HTML Capabilities (Unit 3)
-HTML can be debugged in browser developer tools which reveals a website's code and performance.
-HTML attributes are the extra functionality an element can have. Some can work with multiple elements not all.
-There are 4 main attributes: 1- Classes 2- ID's 3- Language 4- Direction
- There are extra attributes ensuring all users, including people living with disabilites, access the website such as ARIA Roles.

## Week 1: HTML Navigation And Linking (Unit 4)
-HTML linking is not a complex task but has a big impact on how we navigate the web.
-Links are created using anchor tags (a) which has an href attribute to specify the url.
-For a link or website to be secure it must have HTTPS instead HTTP.
-Absolute url's gives us the full url directory while relative url's point to a link on the same page or project.

## Week 2: HTML Working with Graphics (Unit 5)
-Images in HTML are added using the img tag which includes a src, alt, height or weight attribute
-ALT attributes describes the image when the image is unable to load.
-There are different image formats: gif (compresses illustrations with large areas of same color); svg(logos, icons and other illustrations); jpg(compress photos); png(transparency in a photo)
-Images can also be set to be repsonsive which is the ability to appear in different screen sizes.
-Images contain figure captions and figure elements which is easier for interactive graphic.

## Week 2: Working With Media (Unit 6)
-Unlike the img element the audio element has a closing tag, which is modern, also includes the src attribute.
-The controls attribute allows us to add play/pause/volume features without building it from scratch.
-We can also provide fallback text to audio for cases when audio does not load.
-The video element is similar to the audio element however videos are encoded differently and adapts to different resolutions in the browser.
-Captions and descriptions can also be added in video elements to understand the content.
-Other media can be embedded in a HTML website using the <iframe> tag

## Week 2: HTML Content Identification (Unit 7)
-HTML has an atribute (lang) that can use any language in the world for the browser to understand content.
-You could use different languages on the same HTML document by using block quote elements.
-The direction of the work flow is important as different languages flow in different directions.
-We are also able to insert the characters for a specific language using the UTF element.
-HTML groups elements using a div tag and groups elements within a line using a span tag.

## Week 2: HTML Intergration (Unit 8)
-A standard HTML begins with a doctype statement indicating the period of the HTML file.
-The document is enclosed in a <html> tag and there are two main parts: the head and body section.
-The head consists of the meta tag, title of page and other linkage sites.
-The meta element serves to inform the browser that the layout has been adjusted and describe the site to appear in search engines.
-The link connects assets needed to be loaded on the page (CSS files, fonts, icons etc.)
-The script tag can also be used in the head of the document structure.
-The typical structure consists of 6 main elements.
-1.Main: this element is used once per webpage, indicating where the main content is
-2.Header: this element is found at the top of most web pages including a logo, site name and navigation.
-3.Footer: this element signifies extra things to do, regardless of position 
-4.Article: this element wraps around any type of content with a title, subtitle, author's name and publication date.
-5.Section: this element marks sections of the page content and dividing topics in a webpage.
-6.Aside: this element is for content on the side of the webpage e.g. sidebar information but not part of the main content.

## Week 3: HTML Working with Forms and Interactive Elements (unit 9)
-Forms are used for different cases, in HTML they have a built-in power of the browser that detects forms.
-By using form elements, this allows one to use forms across all devices and hardware.
-A form is created by the form element or tags
-They consists of a fields, input, label and a button for submission.
-Input elements don't only take text but numbers and emails too by addinf the type attribute.
-The inputs contain placeholders that inform the user what to type in the textbox.
-A value attribute also ensures that the correct value that is wanted on the form is typed in.
-Depending on the type of attribute use, forms can have various inputs such as radio buttons and lists.

## Week 3: Organizing Tabular Information in HTML (unit 10)
-When HTML content is in a form of a table it is best to use the table element.
-HTML tables makes the content accessible,reusable and findable.
-Tables can also be styled using CSS for layout for different screen sizes.
-There are several elements that are used in an HTML table: TH, TR and TD
-Similarly to images, tables can also contain captions.

## Week 3: Introduction To CSS(unit 1)
-CSS is a style sheet for HTML web pages.
-CSS has a selector and declaration block.
-Selector is specific for a pattern HTML, if pattern matches CSS code in declaration blocks is applied.
-Cascading part is when multiple styles are applied to the same pattern.
-Each style has two parts: property and value.
-There is an element selector (e.g. select all paragraphs on page)
-There is a class selector (e.g specific to an element)
-The same style can be applied to different selectors (group selectors)
-With a descendant selector we can select list items that are descendants of either an ordered or unordered list.
-Code can also be commented out on CSS to see the effect of removing styles.

## Week 3: Adding CSS colors(unit 2)
-CSS can also write comments just like HTML.
-The first selector is the element selector in CSS that selects all elements marked
-CSS can detect a class by writing a fullstop and opening brackets to declare code
-Style declarations can be placed in any order.
-Elements with similar styles can be grouped together to apply the same style.
-Other elements acts as descendants and can be selected as well.


## Week 4: CSS Images and Colors(unit 3)
-In CSS choosing a color pallette is important to keep your styling similar
-Colors are given in hex codes in CSS where you can specify a color one needs.
-The types of color formats are RGB, HSL and HSLA
-Changing background colors and images are possible with the background color and image properties.
-Images are found in different formats on the web: PNG, GIF & JPEG all serving different purposes.
-Background images contain a url value which specifies the location of the image.

## Week 4: CSS Boxes, Types and Sizes(unit 4)
-Fonts and spacing play a huge role in making HTML pages attractive.
-There are different stack for fonts but mainly Serif and Sans serif are popular.
-Fonts are applied on the CSS sheet to make things decent and readable.
-We are also able to change the font size and overide the default sizes of the browser.
-There is absolute sizing(pixels,points), remain the same regardless of screen size.
-Relative sizing can adjust based on the page size. (rem)
-The box model allows us to adjust the height and width of the content inside margins, paddings and borders.

## Week 4: Advanced CSS Properties and Concepts(unit 5)
-Typically links are blue and purple once you click on them, with CSS you can style them to default colors.
-We do this by targetting the a tag and changing its color.
-In CSS a concept called inheritance plays a huge role by inheriting styles of previously declared elements.
-When debugging CSS it is important to look at the selectors and declarations made are carefully applied.







