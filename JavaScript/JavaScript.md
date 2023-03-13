# JavaScript

## **Variable**

- Var
    - Variables are container of a datatype values.
    - Every data type should contain a unique name(identifier).
        
        ```jsx
        <!DOCTYPE html>
        <html>
        <body>
        <h1>JavaScript Variables</h1>
        <p>In this example, x, y, and z are variables.</p>
        <p id="demo"></p>
        <script>
        var x = 5;
        var y = 6;
        var z = x + y;
        document.getElementById("demo").innerHTML =
        "The value of z is: " + z;
        </script>
        </body>
        </html>
        ```
        
- Const
    - constant variable are used mostly for a constant data type that cannot be changed.
    - And we use const to declare a constant datatype.
        
        ```jsx
        <!DOCTYPE html>
        <html>
        <body>
        
        <h1>JavaScripta Variables</h1>
        
        <p>In this example, price1, price2, and total are variables.</p>
        
        <p id="demo"></p>
        
        <script>
        const price1 = 5;
        const price2 = 6;
        let total = price1 + price2;
        document.getElementById("demo").innerHTML =
        "The total is: " + total;
        </script>
        
        </body>
        </html>
        ```
        
- Let
    - when using let in variable ww use it to change the value of the datatype of a default value.
    - use the example in constant.

## **Datatype**

- JavaScript has 8 Datatype
    1. String
        - In our pervious class we have learned that we use string to write multiple character in one line of code.
        - And as we write the code we must use double quote(”quote”).
            
            ```jsx
            <!DOCTYPE html>
            <html>
            <body>
            
            <h2>JavaScript Strings</h2>
            
            <p>Strings are written with quotes. You can use single or double quotes:</p>
            
            <p id="demo"></p>
            
            <script>
            let carName1 = "Volvo XC60";
            let carName2 = 'Volvo XC60';
            
            document.getElementById("demo").innerHTML =
            carName1 + "<br>" + 
            carName2; 
            </script>
            
            </body>
            </html>
            ```
            
    2. Number
        - We can use number in the datatype or variable to assign some value of x.
            
            ```jsx
            // With decimals:
            let x1 = 34.00;
            
            // Without decimals:
            let x2 = 34;
            ```
            
    3. BigInt
        - JavaScript bigint variables are used to store big integer values that are too big to be represented by a normal JavaScript number.
            
            ```jsx
            <!DOCTYPE html>
            <html>
            <body>
            
            <h1>JavaScript Numbers</h1>
            <h2>Integer Precision</h2>
            
            <p>Integers (numbers without a period or exponent notation) are accurate up to 15 digits:</p>
            
            <p id="demo"></p>
            
            <script>
            let x = 999999999999999;
            let y = 9999999999999999;
            document.getElementById("demo").innerHTML = x + "<br>" + y;
            </script>
            
            </body>
            </html>
            ```
            
    4. Boolean
        - JavaScript can only have one of two values:
            - Yes / No
            - True / False
            - On / Off
                
                ```jsx
                <!DOCTYPE html>
                <html>
                <body>
                
                <h2>JavaScript Booleans</h2>
                <p>Display the value of Boolean(10 > 9):</p>
                
                <p id="demo"></p>
                
                <script>
                document.getElementById("demo").innerHTML = Boolean(10 > 9);
                </script>
                
                </body>
                </html>
                
                **Output:**
                JavaScript Booleans
                Display the value of Boolean(10 > 9):
                
                true
                ```
                
    5. Undefined
        - It is a datatype that indicates a variable has not been assigned a value.
        - When a variable is declared without a value, it is assigned undefined.
            
            ```jsx
            <!DOCTYPE html>
            <html>
            <body>
            
            <h2>JavaScript Undefined</h2>
            
            <p id="demo"></p>
            
            <script>
            let car;
            document.getElementById("demo").innerHTML =
            "The value of car is " + car;
            </script>
            
            </body>
            </html>
            
            ```
            
    6. Null
        - Null is a datatype in JavaScript that represents a variable with no value. It is different from undefined because null is explicitly assigned to a variable by a programmer, whereas undefined is assigned by the system.
    7. Symbol
        - Symbol is a primitive datatype in JavaScript that is used to create unique identifiers for objects. Symbols are created using the `Symbol()` function, and each symbol created is unique and immutable. Symbols are often used as property keys in objects, to avoid naming conflicts with other properties. For example:
            
            ```jsx
            const sym = Symbol("description");
            const obj = {
              [sym]: "This is a symbol description",
              name: "John",
              age: 30
            };
            
            console.log(obj[sym]); // Output: "This is a symbol description"
            
            ```
            
        - In the above example, `sym` is a symbol with the description "description". It is used as a property key in the `obj` object, along with other properties like `name` and `age`.
    8. Object
        - Object is a datatype in JavaScript that is used to store collections of data, such as key-value pairs. Objects are created using the `{}` syntax, and can contain any number of properties, each with its own key and value. For example:
            
            ```jsx
            const person = {
              name: "John",
              age: 30,
              hobbies: ["reading", "swimming", "traveling"],
              address: {
                street: "123 Main St",
                city: "New York",
                state: "NY"
              }
            };
            
            console.log(person.name); // Output: "John"
            console.log(person.hobbies[0]); // Output: "reading"
            console.log(person.address.city); // Output: "New York"
            
            ```
            
        - In the above example, `person` is an object with properties like `name`, `age`, `hobbies`, and `address`. The `hobbies` property is an array, and the `address` property is another object with its own properties like `street`, `city`, and `state`.

## Data Structure

- Data structures are techniques for storing and organizing data that make it easier to modify, navigate, and access. Data structures determine how data is collected, the functions we can use to access it, and the relationships between data.
- JavaScript has primitive and non-primitive data structures.
    - **Primitive data structures** and data types are native to the programming language. These include boolean, null, number, string, etc.
    - **Non-primitive data structures** are not defined by the programming language but rather by the programmer. These include linear data structures, static data structures, and dynamic data structures, like queue and linked lists.
        1. Array
            - The most basic of all data structures, an array stores data in memory for later use. Each array has a fixed number of cells decided on its creation, and each cell has a corresponding numeric index used to select its data. Whenever you’d like to use the array, all you need are the desired indices, and you can access any of the data within.
            - **Advantages**
                - Simple to create and use.
                - Foundational building block for complex data structures
            - **Disadvantages**
                - Fixed size
                - Expensive to insert/delete or resequence values
                - Inefficient to sort

## Object

- A JavaScript object is just a collection of named values. These named values are usually referred to as properties of the object.
- An object is similar to an array, but the difference is that you define the keys yourself, such as name, age, gender, and so on.
    
    ```jsx
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="utf-8">
        <title>Creating Objects in JavaScript</title>
    </head>
    <body>
        <script>
        var person = {
            name: "Peter",
            age: 28,
            gender: "Male",
            displayName: function() {
                alert(this.name);
            }
        };
        
        document.write(person.name + "<br>"); // Prints: Peter
        document.write(person.age + "<br>"); // Prints: 28
        document.write(person.gender); // Prints: Male
        console.log(person); 
        </script>
        <p><strong>Note:</strong> Also check out the browser console by pressing the f12 key on the keyboard.</p>
    </body>
    </html>
    
    output:
    
    Peter
    28
    Male
    Note: Also check out the browser console by pressing the f12 key on the keyboard.
    ```
    

## Events

- An event is something that happens when user interact with the web page, such as when he clicked a link or button, entered text into an input box or text area, made selection in a select box, pressed key on the keyboard, moved the mouse pointer, submits a form, etc. In some cases, the Browser itself can trigger the events, such as the page load and unload events.
- There are several ways to assign an event handler. The simplest way is to add them directly to the start tag of the HTML elements using the special event-handler attributes. For example, to assign a click handler for a button element, we can use `onclick`
 attribute, like this:
    
    ```jsx
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="utf-8">
        <title>JavaScript Attaching Event Handlers Inline</title>
    </head>
    <body>
        <button type="button" onclick="alert('Hello World!')">Click Me</button>
    </body>
    </html>
    
    output:
    
    Click ME (Display "Hello World!")
    
    ```
    

## Function

- A function is a group of statements that perform specific tasks and can be kept and maintained separately form main program. Functions provide a way to create reusable code packages which are more portable and easier to debug. Here are some advantages of using functions:
    - Functions reduces the repetition of code within a program.
    - Functions makes the code much easier to maintain.
    - Functions makes it easier to eliminate the errors.
    
    ```jsx
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="utf-8">
        <title>JavaScript Define and Call a Function</title>
    </head>
    <body>
        <script>
        // Defining function
        function sayHello() {
            document.write("Hello, welcome to this website!");
        }
         
        // Calling function
        sayHello(); // Prints: Hello, welcome to this website!
        </script>
    </body>
    </html>
    
    output:
    
    Hello, welcome to this website!
    ```
    

## Condition

- JavaScript also allows you to write code that perform different actions based on the results of a logical or comparative test conditions at run time.
    - There are several conditional statements in JavaScript that you can use to make decisions:
        1. **The if statement**
            - The if statement is used to execute a block of code only if the specified condition evaluates to true.
                
                ```jsx
                <!DOCTYPE html>
                <html lang="en">
                <head>
                    <meta charset="utf-8">
                    <title>JavaScript If Statement</title>
                </head>
                <body>
                    <script>
                    var now = new Date();
                    var dayOfWeek = now.getDay(); // Sunday - Saturday : 0 - 6
                    
                    if(dayOfWeek == 5) {
                        document.write("Have a nice weekend!");
                    }
                    </script>
                    <p><strong>Note:</strong> This example will print "Have a nice weekend!" if the current day is Friday.</p>
                </body>
                </html>
                
                output:
                
                Note: This example will print "Have a nice weekend!" if the current day is Friday.
                ```
                
        2. **The if...else statement**
            - The if-else statement allows you to execute one block of code if the specified condition is evaluates to true and another block of code if it is evaluates to false. It can be written, like this:
                
                ```jsx
                <!DOCTYPE html>
                <html lang="en">
                <head>
                    <meta charset="utf-8">
                    <title>JavaScript If-Else Statement</title>
                </head>
                <body>
                    <script>
                    var now = new Date();
                    var dayOfWeek = now.getDay(); // Sunday - Saturday : 0 - 6
                    
                    if(dayOfWeek == 5) {
                        document.write("Have a nice weekend!");
                    } else {
                        document.write("Have a nice day!");
                    }
                    </script>
                </body>
                </html>
                
                output:
                
                Have a nice day!
                ```
                

## Loop

- Loops are used to execute the same block of code again and again, as long as a certain condition is met. The basic idea behind a loop is to automate the repetitive tasks within a program to save the time and effort. JavaScript now supports three different types of loops:
    1. ****The while Loop****
        - The while loop loops through a block of code as long as the specified condition evaluates to true. As soon as the condition fails, the loop is stopped.
            
            ```jsx
            <!DOCTYPE html>
            <html lang="en">
            <head>
                <meta charset="utf-8">
                <title>JavaScript While Loop</title>
            </head>
            <body>
                <script>
                var i = 1;
                while(i <= 5) {    
                    document.write("<p>The number is " + i + "</p>");
                    i++;
                }
                </script>
            </body>
            </html>
            
            output:
            
            The number is 1
            
            The number is 2
            
            The number is 3
            
            The number is 4
            
            The number is 5
            ```
            
    2. ****The do...while Loop****
        - The do-while loop is a variant of the while loop, which evaluates the condition at the end of each loop iteration. With a do-while loop the block of code executed once, and then the condition is evaluated, if the condition is true, the statement is repeated as long as the specified condition evaluated to is true.
            
            ```jsx
            <!DOCTYPE html>
            <html lang="en">
            <head>
                <meta charset="utf-8">
                <title>JavaScript Do-While Loop</title>
            </head>
            <body>
                <script>
                var i = 1;
                do {
                    document.write("<p>The number is " + i + "</p>");
                    i++;
                }
                while(i <= 5);
                </script>
            </body>
            </html>
            
            output:
            
            The number is 1
            
            The number is 2
            
            The number is 3
            
            The number is 4
            
            The number is 5
            ```
            
    3. ****The for Loop****
        - The for loop repeats a block of code as long as a certain condition is met. It is typically used to execute a block of code for certain number of times.
        - The parameters of the `for` loop statement have following meanings:
            - ***initialization*** — it is used to initialize the counter variables, and evaluated once unconditionally before the first execution of the body of the loop.
            - ***condition*** — it is evaluated at the beginning of each iteration. If it evaluates to `true`, the loop statements execute. If it evaluates to `false`, the execution of the loop ends.
            - ***increment*** — it updates the loop counter with a new value each time the loop runs.
            
            ```jsx
            <!DOCTYPE html>
            <html lang="en">
            <head>
                <meta charset="utf-8">
                <title>JavaScript For Loop</title>
            </head>
            <body>
                <script>
                for(var i=1; i<=5; i++) {
                    document.write("<p>The number is " + i + "</p>");
                }
                </script>
            </body>
            </html>
            
            output:
            
            The number is 1
            
            The number is 2
            
            The number is 3
            
            The number is 4
            
            The number is 5
            ```
