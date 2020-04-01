## Build a server in a React app
    Build a server in a React app that logs 'Take me to warp [port number]!' when you run nodemon.
<details>
<summary>Not sure where to start?</summary>

* To make a server we need a server folder at the root of our project with an index.js file inside. We need to install a package and then implement it in index.js
</details>

<details>
<summary>I'm stuck!</summary>

* Make a server folder at the root of the project. 
* Make an index.js file.
* npm i express and require it into the index.js file. 
* If you're still not sure what to do, reference the node morning review that we've been working on. 
</details>

## Create a controller file with an array to store data and an object to hold the methods for our endpoints
<details>
<summary>Not sure where to start?</summary>

* We need to create a folder in the server folder called controllers, this will hold a file called controller.js. 
* We should have an empty array in this file to hold data in. 
* Our functions for our endpoints will also be in this folder, formatted so we can import them into index.js and access them. 

</details>

<details>
<summary>I'm stuck!</summary>

* controller.js should have a variable declared at the top with an empty array as it's value. We'll use this array to hold data. 
* We are going to write our functions in this file and export them all in an object. We'll do this with ```module.exports ``` and write the functions as methods on the object we're exporting. 

</details>

## Write four endpoints that will add, get, edit and delete people objects (object with first name and last name) in the array in our controller. 

<details>
<summary>Not sure where to start?</summary>

*  We need a post endpoint first, because our array is empty. Write a post endpoint that will pull a person object off ```req.body``` and add it to the array. 
* Now let's a get endpoint that will simply send back the entire array. 
* The put endpoint should be able to take the value of a ```firstName``` property off of ```req.query``` and use it to find the matching person from our people array, then update that person's info with a new object from ```req.body```.
* The delete endpoint should be able to take the value of a ```firstName``` property off of ```req.query``` and use it to find the matching person from our people array, then splice that object out of the array. 

</details>

### If you need more instruction beyond this point reference the morning reviews code. 