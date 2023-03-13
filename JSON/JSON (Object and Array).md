# JSON

## What is JSON?

- JSON stands for **J**ava**S**cript **O**bject **N**otation. JSON is extremely lightweight data-interchange format for data exchange between server and client which is quick and easy to parse and generate.
- Like XML, JSON is also a text-based format that's easy to write and easy to understand for both humans and computers, but unlike XML, JSON data structures occupy less bandwidth than their XML versions.
    - JSON stands for JavaScript Object Notation, and it is a lightweight data interchange format. It is a text-based format that is easy to read and write for both humans and machines.
    - JSON is often used to transmit data between a server and a web application, but it can be used for any application that needs to transmit or store data in a structured format. It is based on a subset of the JavaScript programming language, but it can be used with any programming language.
    - JSON uses a simple syntax that consists of key-value pairs, where the keys are strings and the values can be any valid JSON data type, including numbers, strings, booleans, arrays, and other JSON objects. Here is an example of a simple JSON object:

## **Object**

- This is defined as an unordered collection of key/value pairs (i.e. `key:value`). Each object begins with a left curly bracket `{` and ends with a right curly bracket `}`. Multiple key/value pairs are separated by a comma `,`.
    - A JSON object is an unordered collection of key-value pairs, where the keys are strings and the values can be any valid JSON data type such as a string, number, Boolean, null, array, or another object. It is denoted by curly braces **`{ }`**
     and each key-value pair within the object is separated by a comma.
    - JSON objects are useful for representing complex data structures, such as data from a database or an API response. They can also contain arrays and other objects, making them a powerful way to represent nested data structures.

## Array

- This is defined as an ordered list of values. An array begins with a left bracket `[` and ends with a right bracket `]`. Values are separated by a comma `,`.
    - **A JSON array** is an ordered collection of values, where each value can be a JSON data type such as a string, number, Boolean, null, array, or object. It is denoted by square brackets **`[ ]`** and each value within the array is separated by a comma.
    - JSON arrays are useful for representing lists of data, such as a list of products in an online store or a list of comments on a blog post. They can also contain other arrays and objects, making them a powerful way to represent complex data structures.

JSON is based on two basic structures:

```jsx
**Array JSON**
[  
   { 
     "name": "John",    
     "age": 30,    
     "city": "New York" 
   },  
   {
     "name": "Jane",    
     "age": 25,    
     "city": "Los Angeles"  
   },  
   {    
     "name": "Bob",
     "age": 40,
     "city": "Chicago"  
   }
]
```

- In this example, we have an array containing two objects, each representing a person with their name, age, and city.

JSON is based on two basic structures:

```jsx
**Object JSON**
{
  "name": "John",
  "age": 30,
  "city": "New York"
}
```

- In this example, the object has three key-value pairs: "name" with the value "John", "age" with the value 30, and "city" with the value "New York". The values can be accessed using the key names, and the object can be easily parsed and manipulated by applications that understand JSON.