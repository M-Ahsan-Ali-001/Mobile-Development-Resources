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
console.log(employee);
~~~

# Functions  
 ~~~
 function detail(x,y) {
 console.log("user:",x , "id:",y);
 }
 
 detail("brk101",5567)
 ~~~
 # array
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
 

