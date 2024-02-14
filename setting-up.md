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
When using npm dont load whole libs. Use only this modules thaht you really need!