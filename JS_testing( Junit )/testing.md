# Testing in JavaScript

# JEST test
~~~
function func(strA ,strB) { return  strA.concat(strB)}

expect(func('abc','def')).toBe('abcdef') // testing by giving input and comparing ouput
~~~

# Types of Testing

~~~
// End to End Testing (e2e) : how user migth to interact with our app (slowest, examples = [ WebddriverJS , Protractor , Cypress]). 
// Integration Tesing : how spearate modules are integrated and tested (faster than e2e ,examples = [reactlibrary , enzymes]).
// Unit Testing : it is used to tested code in isolation. ().
~~~
