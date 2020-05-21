<!-- Basic Tags -->
# Basic Tags

## Title & Headings 
* Title
  * ```html
    <title>This is the title!</title>
    ```
* Documents 
  * html (Tab)
* Type of Headings (6)
  * ```html
    <h1>This is the largest heading!</h1>
    ```
  *  ```html
     <h6>This is the smallest heading!</h6>
     ```

## Common syntex
* Paragraph   
  * The text starts with a new line 
    * ```html
      <p>This is another paragraph!</p>
      ```
* Bold (Not in use anymore, replaced by strong)  
  * The text gets bold
    * ```html
      <b>The text gets bold!</b>
      ```
* Strong   
  * The text gets bold
    * ```html
      <strong>The text gets bold!</strong>
      ```
* Italics (em is prefered)
  * The text gets italics
    * ```html
      <i>The text gets italics!</i>
      ```
* Emphasis
  * The text gets italics
    * ```html
      <em>The text gets italics!</em>
      ```
  
# HTML Lists
* Ordered lists
  * ```html
       <ol>
         <li>Red</li>
         <li>Orange</li>
         <li>Yellow
       </ol>
       ```
* Unordered lists
  * ```html
       <ul>
         <li>Red</li>
         <li>Orange</li>
         <li>Yellow
       </ul>
       ```
 * Nested list
   * ```html
     <ol>
      <li>Red</li>
      <li>Orange</li>
      <li>Yellow
       <ul>
        <li>Sunflower</li>
        <li>Banana
         <ol>
          <li>Frozen Banana</li>
          <li>Non-Frozen Banana</li>
         </ol>
        </li>
       </ul>
      </li>
     </ol>
     ```
# HTML Attributes
* Image    
  * Shows the image of the link (link can be an url)
    * ```html
      <img src = "dog.jpg">
      ```
* Links   
  * Go to the link 
    * ```html
      <a href="www.google.com">Click me to go to Google</a>
      ```

# Tables

<!--  Name  Age
============
Rusty   2
Wyatt   13
-->

Table sample (Without styling无网格)（添加网格将第一行替换为```<table border="1">```）
* ```html
       <table>
         <thead>
            <tr>
              <th>Name</th> 	
              <th>Age</th> 	
              <th>Breed</th> 	
            </tr>
         </thead>
         <tbody>
           <tr>
             <td>Rusty</td>
             <td>2</td>
             <td>Mutt</td>
           </tr>
           <tr>
              <td>Wyatt</td>
              <td>13</td>
              <td>Golden</td>
           </tr>
         </tbody>
       </table>
    ```

### Pokemon table sample
[Pokemon table sample](https://github.com/ShaoyangYe/Web-Development-Notes/blob/master/HTML%20Files/pokemonSolution.html)

## Command+Shift+D => repeat block of code.
## Command and choose mutiple images and set size for all chosen images 
* like ```<img width="50" src="" >``` 

# Form, Label, Simple Validations 
* Use the ```<form></form>``` tag (Until we cover Back End JS, our forms won't actually do anything)
  * ```html
    <form action="/my-form-submitting-page" method="post">
    <!-- All our inputs will go in here -->
    </form>
    ```
  * action - the URL to send form data to
  * method - the type of HTTP request 
* Use the ```<input>``` tag
  * ```html
    
    <input type="text">

    <input type="date">

    <input type="color">

    <input type="file">

    <input type="checkbox">
    ```
* Use the ```<label></label>``` tag
  * ```html
    <form action="/sign-in-url" method="post">
        <!-- Using "for" and  "id" attributes -->
        <label for="username">Username:</label>
        <input id="username" type="text">
        <label for="password">Password:</label>
        <input id="password" type="password">
        <button>Login</button>
    </form>
    ```
* Write Simple Validations
  * ```html
    <form action="/sign-in-url" method="post">
      <label for="email">Email:</label>
      <input id="email" type="email" required>
      <label for="password">Password:</label>
      <input id="password" type="password" required>
      <button>Login</button>
    </form>
    ```
  * The 'required' attribute validates that an input is not empty
  * There are also type validations.  Try changing "type" from "text" to "email"
