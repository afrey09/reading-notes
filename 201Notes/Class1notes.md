How the Web Works
    Clients and Servers - A client requests information from a server, the server then responds by to the client with the information requested

Toolbox parts
    internet connection - Allows you to send and receive data on the web
    
    tcp/ip - Defines how the data should travel across the internet. It is like the transport mechanism
    
    dns - The address book for websites. The DNS is looked at by the broswer to find the website's IP address in order to retrieve the actual website. It must find which server the website lives on to it can then send HTTP messages to the right place.
   
    http - Hypertext Transfer Protocol - used to define a language for clients and servers to speak to each other.

    component files - What websites are made up of.. The 2 main paths:
        code files - websites are built primarily from HTML, CSS and Javascript
        assets - the collective name for all the other stuff that makes up websites such as images, music, videos, word doucments and PDFs

The Process

The browser goes to the DNS server, and finds the real address of the server that the website lives on (you find the address of the shop).
The browser sends an HTTP request message to the server, asking it to send a copy of the website to the client (you go to the shop and order your goods). This message, and all other data sent between the client and the server, is sent across your internet connection using TCP/IP.
If the server approves the client's request, the server sends the client a "200 OK" message, which means "Of course you can look at that website! Here it is", and then starts sending the website's files to the browser as a series of small chunks called data packets (the shop gives you your goods, and you bring them back to your house).
The browser assembles the small chunks into a complete web page and displays it to you (the goods arrive at your door — new shiny stuff, awesome!).

How HTML, CSS and JS are "parsed" in a browser

The browser parses the HTML file first, and that leads to the browser recognizing any <link>-element references to external CSS stylesheets and any <script>-element references to scripts.
As the browser parses the HTML, it sends requests back to the server for any CSS files it has found from <link> elements, and any JavaScript files it has found from <script> elements, and from those, then parses the CSS and JavaScript.
The browser generates an in-memory DOM tree from the parsed HTML, generates an in-memory CSSOM structure from the parsed CSS, and compiles and executes the parsed JavaScript.
As the browser builds the DOM tree and applies the styles from the CSSOM tree and executes the JavaScript, a visual representation of the page is painted to the screen, and the user sees the page content and can begin to interact with it.

How to find images

    Go to google images and search for an image. Right click and select "save as". Ensure you select tools, usage rights and creative common licenses to make sure you are using images that are not copyrighted.

How to Create a String vs a Number in JS

    let myVariable = 'sue' . The quote marks signify that it is a string
    let myVariable = 9 . Number's do not have quote marks around them    

Variables are containers that store values. You retrieve the value by calling the variable name. They are needed to do anything interesting in programming. 

DNS = Domain Name Server
    Used to match up with an IP address with a web address

Website Design and Process

    Plan
    Sketch out design
    Choose Assets

Javascript rundown - https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/JavaScript_basics

    /* comments go between */
    No line breaks, use //

HTML

An HTML attribute contains extra information about an element that won't appear in the content. EX. <p class="editor-note">My cat is very grumpy </p>

Anatomy of an HTML element
    opening tag <p> 
    content My cat is very grumpy
    closing tag </p>

Difference between <article> and <section>

    Article encloses a block of related content that makes sense on its own without the rest of the page (e.g a single blog post)

    Section is for grouping together a single part of a page that constitutes one single piece of functionality or a theme. Begin each section with a heading. You can break article's up into different sections or vice versa, depending on the context

Typical Elements of a Website

    Header
    Navigation bar
    Main content
    Sidebar
    Footer

Metadata is used by search engines to recognize various information and make sense of your webpage. It is using the search engine's own language to determine which pages to pull up first and what information to display

<meta> can be used to specify the document's character encoding - the character set that the document is permitted to use.

Website Design

The first step to designing a website is project ideation and answering the qeustions, what do I want the website to accomplish, will the website help me reach my goals and what needs to be done, and in what order, to achieve my goals?

The most important question is what do I want my website to accomplish

Semantics

Using <h1> gives the meaning of a top level heading on a page. <Span> on the other hand will make it look like a top level heading but without the semantic value.

Benefits of semantic tags:
    Search engines will consider its contents as important keywords to influence the page's search rankings (see SEO)
    
    Screen readers can use it as a signpost to help visually impaired users navigate a page
    
    Finding blocks of meaningful code is significantly easier than searching through endless divs with or without semantic or namespaced classes

    Suggests to the developer the type of data that will be populated

    Semantic naming mirrors proper custom element/component naming

Javascript

   Two things that require javascript in a browser is animated images and controlled multimedia. Without javascript, the browser does not have the language needed to implement such effects.

   To add Javascript to an HTML document, you must use the <script> element
