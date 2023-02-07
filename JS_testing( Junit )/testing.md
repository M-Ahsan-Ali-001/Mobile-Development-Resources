# Testing in JavaScript

# JEST Framework (for Javascript)
~~~
function func(strA ,strB) { return  strA.concat(strB)}

expect(func('abc','def')).toBe('abcdef') // testing by giving input and comparing ouput

//Code-Coverage: tell about how much code is tested.
~~~
# Mocking
~~~
//unit testing is stand-alone 
//used to avoid bottleneck 
//used to ship features faster (front-end can be developed first)
//facilitate asyncronous code
 ~~~
# Snapshot testing
~~~
// used by developers to verify that there are no regressions in the DOM

~~~
 
 
 
# Types of Testing

~~~
// End to End Testing (e2e) : how user migth to interact with our app (slowest, examples = [ WebddriverJS , Protractor , Cypress]). 
// Integration Tesing : how spearate modules are integrated and tested (faster than e2e ,examples = [reactlibrary , enzymes]).
// Unit Testing : it is used to tested code in isolation. ().
~~~
# Adding jest to your project folder
~~~
// all these commands needs to be run in terminal 
// npm init -y (used to generate a package. json file for your JavaScript project.)
// npm install -save-dev jest (installing jest)
//npm run test (to execute test)
~~~
