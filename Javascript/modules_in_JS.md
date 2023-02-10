# Default Export
~~~
export default function addNumb(a ,b) { return a + b} //method - 1.
export default addNumb; //method - 2

//exporting  more than one function

function addNumb(a ,b) { return a + b}
function add3umb(a ,b , c) { return a + b +c };
export {addNumb , add3umb};

~~~

# Default Import
~~~
import addTwo from "./addTwo" //method - 1
import { addTwo } from "./addTwo" //method - 2 
~~~
