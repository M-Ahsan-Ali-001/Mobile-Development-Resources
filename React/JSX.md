# Function
~~~

// JSX is the combination of HTML and JavaScript

function Header() {
let title = "Head";
return (

<div  class="header">
<h1>{ title }</h1>
</div>
)

}

// export default Header;
// <Header/> is used to invoke the the function

~~~

# Arrow Function
~~~

const name = (props) => { return <h1>props.test</h1>} // method - 1 
const name = props => { return(<h1>props.test</h1>)} // method - 2  

~~~

# Event Listener
~~~
onClick= {evenHandler} // this is used on click method
~~~
# Button 
~~~
function nameFn(props)
{
let func1 = (prop)=> {console.log('clicked')} // expression function
let func2 = (prop) => console.log('second-method')
function fnc3 (){
console.log('third-method')
 } 

return (

<button onClick="fun1">
Click Me
</button>

)
}

~~~
# Hooks
~~~
// used for handling dynamic events
import {usedState} from react // it must be added othewise hooks would not work
function hookPrac(){
let hold = 0;
let [valueShow , setValue] = useState('string') // can tak number ,string  ( assing string to valueShow)
let funcIncr = (props )=> {
hold =  valueShow + 1
setValue(hold) // it is use to change the value of the valueShow

    }
return(
<button onClick={}>  
</button>
)

}


~~~

# Bablejs
~~~
// Bablejs is a compiler used to transpile JS so that browser is able to understand.
~~~
