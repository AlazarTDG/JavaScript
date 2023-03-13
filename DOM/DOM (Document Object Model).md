# DOM (Document Object Model)

## DOM

- DOM for short, is a platform and language independent model to represent the HTML or XML documents. It defines the logical structure of the documents and the way in which they can be accessed and manipulated by an application program.
- In the DOM, all parts of the document, such as elements, attributes, text, etc. are organized in a hierarchical tree-like structure; similar to a family tree in real life that consists of parents and children. In DOM terminology these individual parts of the document are known as *nodes.*
- To understand this more clearly, let's consider the following simple HTML document:
    
    ```jsx
    <!DOCTYPE html>
    <html>
    <head>
        <title>My Page</title>
    </head>
    <body>
        <h1>Mobile OS</h1>
        <ul>
            <li>Android</li>
            <li>iOS</li>
        </ul>
    </body>
    </html>
    ```
    
- The above HTML document can be represented by the following DOM tree:

![Untitled](DOM%20(Document%20Object%20Model)%20f7603e74dd784acf89e50a3cb068dacf/Untitled.png)

## ****DOM Selectors****

- Selecting the Topmost Elements
    - The topmost elements in an HTML document are available directly as `document`
     properties. For example, the `[<html>](https://www.tutorialrepublic.com/html-reference/html-html-tag.php)` element can be accessed with  `document.documentElement` property, whereas the `[<head>](https://www.tutorialrepublic.com/html-reference/html-head-tag.php)` element can be accessed with `document.head` property, and the `[<body>](https://www.tutorialrepublic.com/html-reference/html-body-tag.php)` element can be accessed with  `document.body` property.
        
        ```jsx
        <!DOCTYPE html>
        <html lang="en">
        <head>
            <meta charset="utf-8">
            <title>JS Select Topmost Elements</title>
        </head>
        <body>
            <script>
            // Display lang attribute value of html element
            alert(document.documentElement.getAttribute("lang")); // Outputs: en
            
            // Set background color of body element
            document.body.style.background = "yellow";
            
            // Display tag name of the head element's first child
            alert(document.head.firstElementChild.nodeName); // Outputs: meta
            </script>
        </body>
        </html>
        ```
        
- Selecting Elements by ID
    - You can select an element based on its unique ID with the `getElementById()` method. This is the easiest way to find an HTML element in the DOM tree.
    - The following example selects and highlight an element having the ID attribute `id="mark"`.
        
        ```jsx
        <!DOCTYPE html>
        <html lang="en">
        <head>
            <meta charset="utf-8">
            <title>JS Select Element by ID</title>
        </head>
        <body>
            <p id="mark">This is a paragraph of text.</p>
            <p>This is another paragraph of text.</p>
        
            <script>
            // Selecting element with id mark 
            var match = document.getElementById("mark");
             
            // Highlighting element's background
            match.style.background = "yellow";
            </script>
        </body>
        </html>
        ```
        
- Selecting Elements by Class Name
    - Similarly, you can use the `getElementsByClassName()` method to select all the elements having specific class names. This method returns an array-like object of all child elements which have all of the given class names. Let's check out the following example:
        
        ```jsx
        <!DOCTYPE html>
        <html lang="en">
        <head>
            <meta charset="utf-8">
            <title>JS Select Elements by Class Name</title>
        </head>
        <body>
            <p class="test">This is a paragraph of text.</p>
            <div class="block test">This is another paragraph of text.</div>
            <p>This is one more paragraph of text.</p>    
        
            <script>
            // Selecting elements with class test
            var matches = document.getElementsByClassName("test");
                
            // Displaying the selected elements count
            document.write("Number of selected elements: " + matches.length);
             
            // Applying bold style to first element in selection
            matches[0].style.fontWeight = "bold";
                
            // Applying italic style to last element in selection
            matches[matches.length - 1].style.fontStyle = "italic";
                
            // Highlighting each element's background through loop
            for(var elem in matches) {  
                matches[elem].style.background = "yellow";
            }
            </script>
        </body>
        </html>
        ```
        
- Selecting Elements by Tag Name
    - You can also select HTML elements by tag name using the `getElementsByTagName()`
     method. This method also returns an array-like object of all child elements with the given tag name.
        
        ```jsx
        <!DOCTYPE html>
        <html lang="en">
        <head>
            <meta charset="utf-8">
            <title>JS Select Elements by Tag Name</title>
        </head>
        <body>
            <p>This is a paragraph of text.</p>
            <div class="test">This is another paragraph of text.</div>
            <p>This is one more paragraph of text.</p>   
         
            <script>
            // Selecting all paragraph elements
            var matches = document.getElementsByTagName("p");
                
            // Printing the number of selected paragraphs
            document.write("Number of selected elements: " + matches.length);
             
            // Highlighting each paragraph's background through loop
            for(var elem in matches) {  
                matches[elem].style.background = "yellow";
            }
            </script>
        </body>
        </html>
        ```