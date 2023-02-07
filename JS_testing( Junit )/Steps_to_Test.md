# Step-1
~~~

// RUN all these commands needs  in terminal 
// npm init -y (used to generate a package. json file for your JavaScript project.)
// npm install -save-dev jest (installing jest)
//npm run test (to execute test)
~~~

# Step-2
~~~
//file name : 'file-name'.js
//make file and make a function in that file
function addFive(val)
{
return val + 5
}

module.exports = addFive // this is used to pass function to other files in same projet older
// save this file
// run 'npm install -save-dev jest' (installing jest)
// open 'package.json' find script, in this change text  to 'jest'and save the file 
// run 'npm  run test'
~~~
# Step-3
~~~
//file name : 'file-name'.test.js
const addFive = require('./addFive') // this is used to call the addFive function
test('name of the test :',()=>{
expect(1).toBe(6);

})
//save this file and run `npm run test`
~~~
