# JSON Storage

## JSON Session

- JSON can be used with web storage APIs like **`sessionStorage`** to store data on the client side. **`sessionStorage`** is a type of web storage that allows you to store key/value pairs for a session. Data stored in **`sessionStorage`** is only available within the current browser tab or window and is cleared when the tab or window is closed.
- Here's an example of using **`sessionStorage`** with JSON:
    
    ```jsx
    // Set data in sessionStorage
    const data = {name: 'John', age: 30, city: 'New York'};
    sessionStorage.setItem('user', JSON.stringify(data));
    
    // Get data from sessionStorage
    const userData = JSON.parse(sessionStorage.getItem('user'));
    console.log(userData.name); // Output: John
    
    // Remove data from sessionStorage
    sessionStorage.removeItem('user');
    ```
    
- In this example, we first create an object called **`data`** with some key/value pairs. We then use **`JSON.stringify`** to convert the object into a JSON string and store it in **`sessionStorage`** using **`setItem`**.
- To retrieve the data, we use **`JSON.parse`** to convert the JSON string back into an object and assign it to a variable called **`userData`**.
- Finally, we remove the data from **`sessionStorage`** using **`removeItem`**.
- I hope this helps! Let me know if you have any other questions.

## JSON Local

- JSON can also be used with the **`localStorage`** API to store data on the client-side. **`localStorage`** works in a similar way to **`sessionStorage`**, but the data stored in **`localStorage`** persists even after the browser is closed.
- Here's an example of using **`localStorage`** with JSON:
    
    ```jsx
    // Set data in localStorage
    const data = {name: 'John', age: 30, city: 'New York'};
    localStorage.setItem('user', JSON.stringify(data));
    
    // Get data from localStorage
    const userData = JSON.parse(localStorage.getItem('user'));
    console.log(userData.name); // Output: John
    
    // Remove data from localStorage
    localStorage.removeItem('user');
    ```
    
- To retrieve the data, we use **`JSON.parse`** to convert the JSON string back into an object and assign it to a variable called **`userData`**.
- Finally, we remove the data from **`localStorage`** using **`removeItem`**.
- In this example, we first create an object called **`data`** with some key/value pairs. We then use **`JSON.stringify`** to convert the object into a JSON string and store it in **`localStorage`** using **`setItem`**.