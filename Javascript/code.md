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
designation: "Manager"
}

console.log(employee);
employee.salary = "14000$";

employee['address'] = "Taxes";
employee["years"] = function() { console.log(5);}

console.log(employee);
employee.years();
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
# Recurssion
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
