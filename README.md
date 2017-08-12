# A-WHOLE-GUIDE-TO-JAVASCRIPT-
This guide contains all Javascript concept made into a small HTML program .
//VIGHNESH TIWARI , AIT PUNE , INDIA 
//GITHUB PROFILE : CR7VIGGY
<html>
<head>
</head>
<body>
<script type = "text/javascript">
/*adding comments in javascript*/
document.write("hello java script i m on u right now");

var x = 20;
var y = "i m in love with u javascript\n";
var z = "u r so awesome";
var m = "parameterized function";
var n = "of two variables";
document.write(y+z+"i love u"+x+"times");
/*non parameterized function in javascript*/
function fun()
{
	alert("you are done with alert funtion also .CONGRATS!!");
}
fun();
/*parameterized funcion in javascript*/
function pfun(m,n)
{
	document.write("you are in a "+m+n);
}
pfun(m,n);

/*creating a calculation in javascript*/
function cal()
{
var x = prompt("enter x");
var y = prompt("enter y");
x = parseInt(x);
y = parseInt(y);
var z = x+y;
document.write(z);
}
/*else if using a function*/
function ifelse()
{
var x = prompt("enter a value");
x = parseInt(x);
if(x == 0)
document.write("oops you have entered zero");
else
document.write("correct value");
}

/*switch statements*/
function switchstat()
{
	var x = prompt("enter 1 : say hi \n enter 2 : say bye");
	x = parseInt(x);
	switch(x)
	{
		case 1 : document.write("hi");break;
		case 2 : document.write("bye");break;
	}
}

/*loop statements*/
function loop()
{
	var x = prompt("enter x");
	x = parseInt(x);
	var sum = 0;
	sum = parseInt(sum);
	for(i = 0 ; i  <= x ; i++)
	{
		sum = sum + x;
	}
	document.write("sum till entered no. is:"+sum);
}
/*creating objects in javascript*/
function person()
{
	var car = {type:"Fiat", model:"500", color:"white"};
	document.write(car.type+car.model+car.color);
}
/*arrays in javascript*/
function arr()
{
	var x = prompt("enter array size");
	x = parseInt(x);
	var arr = [];
	for(var i = 0; i < x; i++)
    arr.push(prompt("Enter a number"));
	alert("full array : "+arr.join(' ,'));
}
/*array sorting in javascript*/
function arrsort()
{
	var x = prompt("enter array size");
	x = parseInt(x);
	var arr = [];
	for(i = 0 ; i < x ; i++)
	{
		arr.push(prompt("enter a no."));
	}
	for(i = 0 ; i < x ; i++)
	{
		arr.sort(function(a,b){return a-b})
	}
	alert("sorted array :"+arr.join(' ,'));
}
/*math random function*/
function random()
{
	document.write(Math.random());
}
/*displaying dates in javascript*/
function dates()
{
	document.write(Date());
}
/*using boolean function*/
function bool()
{
	alert("we ll compare two no.s which is greater\n if first no. is greater than second o/p ll be true else false");
	var x = prompt("enter A");
	var y = prompt("enter b");
	x = parseInt(x);
	y = parseInt(y);
	document.write(prompt(Boolean(x>y)));
}
/*ternary operator in javascript*/
function ternary()
{
	var x = prompt("enter your age");
	x = parseInt(x);
	var y = (x >= 18) ? alert("you are now an adult") :alert("you are not an adult");
}
/*search function in javascript*/
function search()
{
	var x = prompt("enter a word");
	var y = prompt("enter a alphabet to search its position in previous word");
	var n = x.search(y);
	n = parseInt(n);
	alert(n+1);
}
/*replace a string or alphabet*/
function replace()
{
	var x = prompt("enter a word");
	var y = prompt("enter another word");
	var txt = x.replace(x,y);
	alert(txt);
}
</script>
<form>
<input type = "button" value = "CLICK" onclick = "fun()">
<input type = "button" value = "DRAG" onMouseOver = "alert('boom!!')">
</form>
<p>
<input type = "button" value = "CALCULATOR" onclick = "cal()">
<input type = "button" value = "IFELSE" onclick = "ifelse()">
<input type = "button" value = "SWITCH" onclick = "switchstat()">
<input type = "button" value = "LOOP" onclick = "loop()">
<input type = "button" value = "OBJECTS" onclick = "person()">
<input type = "button" value = "ARRAY" onclick = "arr()">
<input type = "button" value = "ARRAY SORT" onclick = "arrsort()">
<input type = "button" value = "RANDOM" onclick = "random()">
<input type = "button" value = "CURRENT DATE AND TIME" onclick = "dates()">
<input type = "button" value = "BOOLEAN" onclick = "bool()">
<input type = "button" value = "TERNARY OPERATOR" onclick = "ternary()">
<input type = "button" value = "STRING SEARCH" onclick = "search()">
<input type = "button" value = "STRING REPLACE" onclick = "replace()">
</p>
</body>
</html>
