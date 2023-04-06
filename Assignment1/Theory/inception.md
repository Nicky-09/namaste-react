What is Emmet ?
Emmet is a set of plugins for text editors that allow you to write HTML and CSS code faster and more efficiently. Emmet provides a shorthand syntax for writing code that expands into full HTML and CSS code.
For example if you type '!' followed by a tab , you will get

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    
</body>
</html>

2. Difference between a Library and a Framework ?
A library is a collection of pre-written code that provides specific functionality that can be called upon by an application. The developer has control over the application and chooses which parts of the library to use, and how to use them. In other words, a library provides a set of tools that the developer can use to build their own application.

A framework, on the other hand, provides a complete structure for building an application. It is a more rigid structure than a library and usually comes with predefined rules and patterns that the developer must follow. The framework defines the architecture, design patterns, and flow of the application. In other words, a framework provides a foundation or skeleton for the application that the developer must build on top of.

In summary, a library provides a set of tools to help developers build their own applications, while a framework provides a complete structure for building an application and the developer builds the application within that structure.
Reactjs is a library and angular is a framework.

3. What is CDN ? Why do we use it ?

A CDN (Content Delivery Network) is a network of servers distributed in different locations around the world that store and deliver content (such as images, videos, CSS, JavaScript, and other static files) to users based on their geographic location. The goal of a CDN is to provide faster and more efficient delivery of web content to users.

When a user requests content from a website, the CDN server closest to the user's location delivers the content, which reduces the distance the content has to travel and speeds up the delivery time. This can improve the performance and speed of a website, especially for users who are located far away from the web server.

CDNs are used for a variety of reasons, including:

Faster content delivery: By caching content on servers around the world, CDNs can deliver content to users more quickly and efficiently.

Reduced server load: By offloading content delivery to the CDN, the web server has less work to do, which can improve the overall performance and reliability of the website.

Improved scalability: CDNs can help websites handle large amounts of traffic, which can be especially important during peak periods.

Lower bandwidth costs: By using a CDN, website owners can reduce their bandwidth costs by offloading some of the traffic to the CDN's servers.

In summary, CDNs are used to improve website performance, reduce server load, improve scalability, and reduce bandwidth costs.

4. Why is React known as React ?
React is named React because of its ability to react to changes in data. React is called React because it was designed to be a declarative, efficient, and flexible JavaScript library for building user interfaces. The name React was chosen because the library was designed to allow developers to "react" to changes in state and data within an application, and to update the user interface in a declarative and efficient manner. React is a JavaScript-based UI development library. Facebook and an open-source developer community run it.React is known as React because of its focus on reactive programming, efficient rendering, and component-based architecture.

5. What is crossorigin in the script tag ?
The crossorigin attribute in the <script> tag is used to specify whether a script file from a different domain should be allowed to access resources on the current page. This attribute is used as a security measure to prevent cross-site scripting (XSS) attacks.

When a script file is loaded from a different domain, the browser will, by default, block it from accessing resources on the current page, such as cookies, local storage, or other sensitive information. This is known as the "same-origin policy".

The crossorigin attribute provides a way to relax this policy and allow the script file to access certain resources on the current page. It has two possible values:

anonymous: This value specifies that the script is loaded from a different domain, but it does not require any special access to resources on the current page.

use-credentials: This value specifies that the script is loaded from a different domain, and it requires access to resources on the current page, such as cookies or local storage. In this case, the server must be configured to allow cross-origin resource sharing (CORS) with the appropriate credentials.
Example
<script crossorigin="anonymous|use-credentials"></script>

6. What is the difference between React and ReactDOM ?
React is a JavaScript library that allows you to build reusable UI components that can be combined to create complex user interfaces. It provides a way to declaratively define the structure and behavior of your UI, and it manages the rendering and updating of your components based on changes in their state or props.

ReactDOM, on the other hand, is a separate library that provides a way to render React components to the DOM (Document Object Model). It provides a set of methods for working with the DOM, such as ReactDOM.render(), which is used to render a React component to a specific container element in the DOM.

React is the library that allows you to define and manage your UI components, while ReactDOM is the library that allows you to render those components to the browser's DOM.

7.What is difference between react.development.js and react.production.js files via CDN ?
The react.development.js file is intended for use during development, as it includes additional error checking and debugging information that can help identify and fix problems in your code. This version is larger in size than the production version, and is not optimized for performance.

The react.production.js file, on the other hand, is a smaller, optimized version of the React library that is intended for use in production environments. It has all of the same functionality as the development version, but with the additional error checking and debugging information removed to improve performance.

When using React via a CDN (Content Delivery Network), you can choose to include either the development or production version of the library depending on your needs. If you're developing a web application and need access to additional debugging information, you can include the development version. However, if you're deploying your application to a production environment, it's recommended that you use the production version for better performance and smaller file size.

8.
async and defer are attributes that can be used with the script tag in HTML to control how and when JavaScript files are loaded and executed on a web page.

async is used to indicate that the script can be executed asynchronously with the rest of the page content, without blocking the rendering of the page. This means that the browser will continue to load and display the rest of the page while the script is being fetched and executed in the background. However, because the script is executed asynchronously, there's no guarantee about the order in which scripts will be executed, or whether the script will finish executing before the rest of the page has loaded.

Here's an example of how to use the async attribute:
<script async src="my-script.js"></script>

defer, on the other hand, is used to indicate that the script should be deferred until after the page has finished parsing. This means that the script will be loaded and executed after the rest of the page content has been loaded and parsed, but before the DOMContentLoaded event is fired. This ensures that the script is executed in the order that it appears in the HTML markup, and that it has access to all of the page content that came before it.

Here's an example of how to use the defer attribute:
<script defer src="my-script.js"></script>

In summary, the async and defer attributes can be used to optimize the loading and execution of JavaScript files on a web page, depending on your specific needs and requirements. async is best used for scripts that don't depend on other scripts or page content, and defer is best used for scripts that need to access page content, but can still be safely deferred until after the page has loaded.




