# Setting up NPM and package.json   

When we start out project we can use terminal and command: `npm init`. It will creat package.json and we can start confing it. 

## Update version of node and npm!

## Local or global installation 

- Locally: NPM will install package only in project folder. 
- Global: NPM will install outside and we can use it everywhere. `-g`

### Locally instal Loadash Libriary 

What is loadash? 
Lodash makes JavaScript easier by taking the hassle out of working with arrays, numbers, objects, strings, etc. Lodash’s modular methods are great for:
- Iterating arrays, objects, & strings,
- Manipulating & testing values
- Creating composite functions

#### Use: `npm i lodash`

#### What happend now? 

##### Package.json updated 
In out package.json we see now: 
```json
"dependencies": {
    "lodash": "^4.17.21" // 4 is major version 17 is minor release - f.e new featurze and 21 is patch release - if they found bugs fixes it will update
  }
```


##### In node-modules loadash appear 

Now we can import to our `scripts.js` like: 
```js
import {without} from 'loadash' // destructuring 

``` 

## Important 
- When using npm dont load whole libs. Use only this modules thaht you really need!

### Dependencies - two types:

#### Dependencies 

-   **Definition**: Dependencies are libraries or packages that a project needs to function correctly in production. These are essential for the application to run as intended for the end-user.
-   **Usage**: They are included in the project's runtime environment and are necessary for the application's core features and functionalities.
-   **Example**: If your project is a web application, dependencies might include frameworks like React or Angular for the frontend, or Express for a Node.js backend.


#### DevDependencies

-   **Definition**: DevDependencies are libraries or packages required only during the development process. They are not needed in the production environment or for the application to run for the end user.
-   **Usage**: These include tools used for compiling/transpiling code, running tests, or managing the build process.
-   **Example**: This might include testing libraries like Jest or Mocha, build tools like Webpack or Gulp, or compilers like Babel.
