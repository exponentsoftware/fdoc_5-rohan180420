## DAY 5
1. Use the countries API to fetch data about countries. (5 pt)

      ```js
      const API_URL = 'https://restcountries.eu/rest/v2/all'
      ```

    Use the countries API to fetch data about countries.

    - How many languages are there in the countries API
    - Find the 15 most spoken languages

    ```sh
    [
    {language: "English", countries: 91}
    {language: "French", countries: 45}
    {language: "Arabic", countries: 25}
    {language: "Spanish", countries: 24}
    {language: "Portuguese", countries: 9}
    {language: "Russian", countries: 9}
    {language: "Dutch", countries: 8}
    {language: "German", countries: 7}
    {language: "Chinese", countries: 5}
    {language: "Serbian", countries: 4}
    {language: "Swahili", countries: 4}
    {language: "Italian", countries: 4}
    {language: "Swedish", countries: 3}
    {language: "Albanian", countries: 3}
    {language: "Croatian", countries: 3}
    ]
    ```

    - Find the 10 most largest countries

    ```sh
    [
    {country: "Russian Federation", area: 17124442}
    {country: "Antarctica", area: 14000000}
    {country: "Canada", area: 9984670}
    {country: "China", area: 9640011}
    {country: "United States of America", area: 9629091}
    {country: "Brazil", area: 8515767}
    {country: "Australia", area: 7692024}
    {country: "India", area: 3287590}
    {country: "Argentina", area: 2780400}
    {country: "Kazakhstan", area: 2724900}
    ]
    ```

2. Explain the following questions in your own words

What is the difference between forEach, map, filter and reduce ? Explain these using your own words
The forEach() method calls a function once for each element in an array, in order.
forEach() is not executed for array elements without values.
The map() method creates a new array with the results of calling a function for every array element.
The map() method calls the provided function once for each element in an array, in order.
map() does not execute the function for empty elements.
map() does not change the original array.
The reduce() method executes a reducer function for each value of an array.
reduce() returns a single value which is the function's accumulated result.
reduce() does not execute the function for empty array elements.
reduce() does not change the original array.
The filter() method creates an array filled with all array elements that pass a test (provided by a function).
filter() does not execute the function for empty array elements.
filter() does not change the original array.


Explain the difference between function declaration and arrow function ?
Regular functions created using function declarations or expressions are ‘constructible’ and ‘callable’. Since regular functions are constructible, they can be called using the ‘new’ keyword. However, the arrow functions are only ‘callable’ and not constructible. Thus, we will get a run-time error on trying to construct a non-constructible arrow functions using the new keyword


Explain the difference between find and findIndex ?
Array.prototype.indexOf() expects a value as first parameter. This makes it a good choice to find the index in arrays of primitive types (like string, number, or boolean).
Array.prototype.findIndex() expects a callback as first parameter. Use this if you need the index in arrays with non-primitive types (e.g. objects) or your find condition is more complex than just a value.


If you like to filter out one object element in an array which method do you like to use: filter or find ? Explain
The filter() method is used to filters all the elements and returns the element that matches and the element that do not match are removed.
The only difference is the filter() method search through all the elements while find() method search through all the child elements only.

Explain the difference of var, let and const when we declare a variable ?
var declarations are globally scoped or function scoped while let and const are block scoped.
var variables can be updated and re-declared within its scope; let variables can be updated but not re-declared; const variables can neither be updated nor re-declared.
They are all hoisted to the top of their scope. But while var variables are initialized with undefined, let and const variables are not initialized.
While var and let can be declared without being initialized, const must be initialized during declaration.