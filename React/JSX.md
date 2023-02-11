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
