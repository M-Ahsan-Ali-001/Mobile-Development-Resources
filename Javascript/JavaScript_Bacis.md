# Print with style 
~~~
var style = "fonst-size : 30px ; color:blue; background-color:green; border: 1px solid red; border-radius:20px; ";
var arr = ["A","C","B"];

for ( var x =0 ; x < arr.length ; x++)
{

console.log("%c" + arr[x],style );
}
~~~

# Loops
~~~

var i = 0;
while (i<12){
console.log(i);
i++;
}

for(var i = 0 ; i<12 ; i++){

console.log(i+1);

}
~~~

# Object Literals 
~~~
var employee ={
name : "user1",
id :3456,
designation: "Manager",
 func: function() {
     this.salary= '5000$'; // accessing inside object variables 
 }   
}

console.log(employee);
employee.salary = "14000$";

employee['address'] = "Taxes";
employee["years"] = function() { console.log(5);}

console.log(employee);
employee.years();
employee.func();
console.log(employee);
~~~
# Object iteration 
~~~
var obj = {
speed:'100-km/hour',
height: '10m'
}

console.log(Objetc.keys(obj)); // prints the all the keys inside obj 
console.log(Objetc.values(obj));// prints the all the values of keys inside obj
console.log(Objetc.entries(obj)); .. prints arrays of both keys and thier values


~~~
# Functions  
 ~~~
 function detail(x,y) {
 console.log("user:",x , "id:",y);
 }
 
 detail("brk101",5567)
 ~~~
 # Array
 ~~~
 function func (a,b,c,){
 var x = [];
 x.push(a);
 x.push(b);
 x.push(c);
 x.pop();
 return x
 }
 
 func(1,3,4);
  
 func("abc",3,4);
 //concat
 var i = ['a','b','c'];
 
 t.concat( ['d','e','f']);
 
 var  j= ['a','b','c'];
 i=i+j
 ~~~
 
# Type Finder 
~~~
typeof(10>2) // boolean
~~~
# Exception Handling
~~~

function add(a,b){
try{
if(typeof(a) != 'number'){
throw new ReferenceError('first is no a number');
}
else if(typeof(b) != 'number'){
throw new ReferenceError('second is no a number');
}
else {
console.log(a+b)
}
}


catch(err)
{
console.log('Error!',err);
}
console.log('Still runs');
}
add(1,'1');
~~~
# Return Single and Multiple values
~~~
function obj (val){
retrun {
   rtn: val,
   sum: val + 4
   }
}
obj (5);
~~~
# Recursion
~~~
function recur(val) {
console.log("Now value of val is : ",val);
if( val === 10){ // === means to compare both variable and also compare there datatype
  return val;
   }
else {
  recur(val+1);
   }

 }

 recur(1);
~~~
# Passing variable to String
~~~
var fontSize= '50px';
var style = `font-size: ${fontSize}`
~~~
# Classes
~~~
class mobile {}
var obj = Object.create(mobile) // method 1 to create object of class
var obj1 = new mobile();
~~~
# constructor
~~~
class a {
  constructor (x,y) {
  this.x =x;
  this.y=y;
      }
  }
  
  class b  {
  constructor (p,e,f) {
    this.p=p;
    this.bf = new a(e,f);

              }
  }
  var obj = new b(1,2,3);
  console.log(obj.bf)
  

~~~

# Inheritence
~~~
class a {
  constructor (x,y) {
  this.x =x;
  this.y=y;
      }
  }
  
  class b extends a {
  constructor (p,e,f) {
   super (e,f);
    this.p=p;
  

              }
  }
  var obj = new b(1,2,3);
  console.log(obj.bf)
~~~

# polymorphism
~~~
// create your classes here
class bike{

ride() {
    console.log('Riding!');
}

}

class accelrator extends bike {
    ride() {
        super.ride() // calling parent func
        console.log('at speed limit');
    }
}
class breakk extends accelrator {

    ride() {
        console.log("break pressed!");
    }
}

var accl = new accelrator ();
var brk =  new breakk();

accl.ride();
brk.ride();
~~~
# Prototype in Classes
~~~
   var proto = Object.getPrototypeOf(this);
~~~
# Default parameter
~~~
function func (number = 10) {
console.log(number * number)
}

~~~

# Types of Varaible in JS 
~~~
var // it can be able to  re-assinged and declared later(normal)

let // it can be able to  re-assinged and declared later(medium)

const // it can not be able to re-assinged and declared later (strict)
~~~
# for in and of loops
~~~

  const obj = {
  speed:100,
  enigne:'on'

  }

  for (proto in obj)
  {
    console.log(proto);
  }

  for (proto of Object.keys(obj)){

    console.log(proto , obj[proto]);
  }
~~~
# forEach on array
~~~
//method # 1 (forEach) 
  const v = ['a' ,'b' , 'c' ,'d']

  function iter( v, idx)
  {
    console.log(`${idx} : ${v} `)
  }

  v.forEach(iter);

  //method #2 (for each)
 
  v.forEach(
    function(v,idx){
      console.log(`${idx} : ${v} `)
    } );
~~~
# filter on array
~~~
 const b = [0,10,23,44,5,66,9];

    console.log(
     b.filter(function(a){
      return a>19})
    )
~~~
# Maps on array
~~~
const b = [0,10,23,44,5,66,9];

    console.log(b.map (function(x){ return x/2}))

~~~

# Maps
~~~
let g = new Map();
g.set(1 ,'test')
g.set(2 ,'test2')
g.set(3 ,'test3')

console.log(g)let g = new Map();
g.set(1 ,'test')
g.set(2 ,'test2')
g.set(3 ,'test3')

console.log(g)
g.get(1);
~~~
# Sets
~~~

// sets remove repitition from array

const arr = ['a' ,'a' ,'b','b','c','c'];

let a =  new Set(arr);
console.log(a);


~~~
# Spread operator 
~~~
var ar =['abc' ,'def' ,'ghk']

function show(n,x,y) {
  console.log(n)
  console.log(x)
  console.log(y)

}
show(...ar)

~~~
# Rest Operator
~~~
// create a mini array 
var ar =[2 ,3 ,4 ,5 ,6]
var ar1 = [7,8,9]
function show(n,...x) {
 return x.map(its => its *n) // its => means passing value in function

}
console.log(show(ar[0],ar[1],ar[2],ar[3],ar[4]))
// output : [6, 8, 10, 12]


//concat array
var ar2 = [...ar , ...ar1]
console.log(ar2)
//output [ 2, 3, 4, 5, 6, 7, 8, 9]
~~~
