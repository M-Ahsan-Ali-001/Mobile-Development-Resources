# print with style 
var style = "fonst-size : 30px ; color:blue; background-color:green; border: 1px solid red; border-radius:20px; ";
var arr = ["A","C","B"];

for ( var x =0 ; x < arr.length ; x++)
{

console.log("%c" + arr[x],style );
}
