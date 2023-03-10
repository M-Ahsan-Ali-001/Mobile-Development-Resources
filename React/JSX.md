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

<button onClick="func1">
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
let count = useRef(0); // it use to directly access DOM  
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
# Prop Drilling
~~~
//prop drilling is a situation where you are passing data from a parent to a child component, then to a grandchild component, and so on, until it reaches a more //distant component further down the component tree, where this data is required.
~~~
# Cotext API
~~~
/*
The React Context API is a way for a React app to effectively produce global variables that can be passed around. This is the alternative to "prop drilling" or moving props from grandparent to child to parent, and so on. Context is also touted as an easier, lighter approach to state management using Redux.

*/

// App.js
import logo from './logo.svg';
import './App.css';
import CtAPi from './Components/CtApi';
import About from './Components/About';
import MealProv from './Components/Ctxt';
import MealList from './Components/MealList';
import {Routes,Route ,Link} from 'react-router-dom'
function App() {
  return (
    <div>
      
      <nav>
        
        <Link to="/">Homepage</Link>
        
        <Link to="/meal">Meal</Link>
        <Link to="/about-me"  >About-Us</Link>

      </nav>
      <Routes>      <Route path="/" element={<CtAPi/> }/>
      <Route path="/about-me" element={<About />}/>
      <Route path="/meal" element={<MealProv><MealList /></MealProv>}/>
      </Routes>

      
    </div>
  )
}

export default App;

// Ctxt.js
import React from "react";

const MealCtx = React.createContext();


const ListM = "beans";//["beans" , "eggs"  , "bread"];

const MealProv = ({children}) =>{

const [meals, setMeal] = React.useState(ListM);
function ChgMe () {
    setMeal("Apples")
}
return (
    <MealCtx.Provider value ={{meals , ChgMe}}>
        {children};
    </MealCtx.Provider>
)

}

export const useMeal = ()=>React.useContext(MealCtx);
export default MealProv;

// MealList
import react, { useMeal } from "./Ctxt";

const MealList = ()=> {
    
   const {meals } =useMeal();
   let style= {marginRight:"auto" , marginLeft:"50%" ,}
    return (
        <div style={style}>
            <h1>All meal</h1>
            <h2>{meals}</h2>
            <button onClick={()=>{console.log("apples")}}> Click</button>
           

            
        </div>
        )

}

export default MealList;

~~~
# Lifting up State
~~~
// we move the useState to parent , component donot have usestate method
~~~
# Reducer
~~~
import React, { useReducer } from "react";

const reducer = (state ,act ) =>{ 
    console.log("re")
        if (act.type==='Driving') return ({money : state.money + 10})
    if (act.type==='refuel') return ({money : state.money - 10})

    return new Error('test');

}


function CtAPi (props) {
    const intiVal = { money:100};

    const [state ,func] =useReducer(reducer, intiVal); //passing value of intiVal obj to  state and passing return of reducer to state
    //func is use to pass type object to reducer 
    return (
<div>
<h1>Cash : {state.money}</h1>
    <div>
    <button onClick={()=>func({type:"Driving"})}>
     Click me
    </button>
    <button onClick={()=>func({type: "refuel"})}>
     refuel
    </button>



     </div>
</div>
   

    )
}

export default CtAPi;
~~~


# Bablejs
~~~
// Bablejs is a compiler used to transpile JS so that browser is able to understand.
~~~

# React Router
~~~
npm i react-router-dom@6 // run in terminal to downlaod and install
// edit idex.js and must add import {BrowserRouter} form 'react-router-dom'
//after that wrap the <App/> like this"<BrowserRouter> <App />></BrowserRouter>"
// now  goto App.js import {Routes,Route,Links} form 'react-router-dom'
// in App.js wrap all the components in Route like this "<Route path ="/"  element={<HomePage/>} >"
// to link to a component we add <Link to="name"> name</Lonk>
// SPA donot naviate is changes the state

// Example 
import logo from './logo.svg';
import './App.css';
import CtAPi from './Components/CtApi';
import About from './Components/About';
import {Routes,Route ,Link} from 'react-router-dom'
function App() {
  return (
    <div>
      
      <nav>
        
        <Link to="/">Homepage</Link>
        <Link to="/about-me"  >About-Us</Link>

      </nav>
      <Routes>      <Route path="/" element={<CtAPi/>}/>
      <Route path="/about-me" element={<About />}/>
      </Routes>

      
    </div>
  );
}

export default App;

~~~

# Conditional Rendering
~~~
(age>18 && age <55)?<Eligble/>: <Not-Eligble/>

true && console.log('This will show') // it will print on screen
false && console.log('This will show') // it will not print on screen
~~~
# Importing an Image
~~~
// rooftops method
import rooftops from './folder and image name'
function Fn(){
return(
<img
height={200}
src={rooftop}
alt="roof-image"
)/>

}

// require method

<img
height={200}
src={require("./folder and image name")}
alt="roof-image"
)/>

// url method
const url = "url of image";
<img
height={200}
src={url}
alt="roof-image"
)/>

~~~


# Media Packages
~~~
//https://github.com/Cookpete/react-player
//terimal code
npm install react-player

// react code
import ReactPlayer from "react-player";
import ReactPlayer from "react-player/youtube";

<ReactPlayer url='https://www.youtube.com/watch?v=ysz5S6PUM-U'
playing={false}
voume={0.5}
/>
~~~
# Audio
~~~
const bird = new Audio(url);
function Ply(){
(bird.paused)?bird.play:bird.pause()

}

~~~
