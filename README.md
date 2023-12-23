# ODD23-24-WT-JavaScript
NAME : P.Jeshwanth Kumar

REFERENCE NUMBER : 212223240114

DEPARTMENT : AIML

# QUESTION 01 :
# AIM :
To Create a form with java script code to calculate electricity bill.

# PROCEDURE :
# STEP 1 :
Create a HTML structure and insert a 'script' tag in the 'head' section for JavaScript.

# STEP 2 :
Inside , create a form with fields for previous and current readings. Add a "Generate Bill" button.

# STEP 3 :
Connect the "Generate Bill" button to a JavaScript function called calc() using onclick.

# STEP 4 :
Write the calc() function to compute the bill based on readings.

# STEP 5 :
Run the code to perform calculations and display the output.

# PROGRAM :
```
<html>
<head>
<script type="text/javascript">
function calc()
{
var prev,curr,units,amt;
prev=Number(document.getElementById("t1").value);
curr=Number(document.getElementById("t2").value);
units=curr-prev;
if(units<=100)
	amt=100;
else if(units>100&&units<=300)
	amt=100+(units-100)*3;
else
	amt=100+600+(units-300)*5;
document.getElementById("t3").value=amt;
}
</script>
</head>
<body>
<h2>Electricity Bill</h2>
<form>
Enter Previous Reading 
<input type="text" id="t1">Enter Current Reading
<input type="text" id="t2">
<input type="button"  onclick="calc()" value="Generate Bill">
<input type="text" id="t3">
</form>
</body>
</html>
```
# OUTPUT :
![Screenshot 2023-12-23 161616](https://github.com/Jeshwanthkumarpayyavula/ODD23-24-WT-JavaScript/assets/145742402/c6d7c27f-72a0-48cb-8aa9-e15122f7cb13)

# RESULT :
Thus the java code to calculate the electricity bill is executed successfully.

# QUESTION 02 :
# AIM :
To Develop a JavaScript program to compute the factorial of a given number without recursion.

# PROCEDURE :
# STEP 1 :
Create a basic 'html' structure. Inside the 'head', add a 'script' tag to include JavaScript.

# STEP 2 :
In the 'body', create a 'form' for user interaction. Include an input field where users can enter a number they want to find the factorial of.

# STEP 3 :
Define a JavaScript function called show(). Inside this function. Initialize a variable fact to 1 to store the factorial result. Retrieve the number entered by the user using getElementById. Use a loop to calculate the factorial of the entered number. Update the result field with the computed factorial value.

# STEP 4 :
Run the code to calculate the factorial of a given number and display the output.

# PROGRAM :
```
<html>
<head>
<script type="text/javascript">
function show()
{
var i, n, fact;
fact=1;
n=Number(document.getElementById("num").value);
for(i=1; i<=n; i++)  
{
fact= fact*i;
}  
document.getElementById("answer").value= fact;
}
</script>
</head>
<body>
<form>
Enter Number: <input type="text" id="num">
<button onclick="show()">Factorial</button>
<input type="text" id="answer">
</form>
</body>
</html>
```
# OUTPUT :
![image](https://github.com/Jeshwanthkumarpayyavula/ODD23-24-WT-JavaScript/assets/145742402/da0f5d1a-86e4-4c26-97b9-d578da489d92)

# RESULT :
Thus the java code for calculating the factorial of the given number has been executed successfully.

# QUESTION 03 :
# AIM :
To construct a JavaScript code to generate ‘N’ prime numbers.

# PROCEDURE :
# STEP 1 :
Begin with the basic 'html' structure. In the 'head', embed a 'script' tag to house the JavaScript code.

# STEP 2 :
Inside the 'body', create a 'form' to capture user inputs. Add two input fields (input type="text") for users to enter a range of numbers: a starting number (n1) and an ending number (n2). Insert a button labeled "Generate" that, when clicked, triggers the JavaScript function to find prime numbers within the range.

# STEP 3 :
Define a JavaScript function named show(). Inside this function Retrieve the lower (n1) and upper (n2) limits entered by the user using getElementById. Implement nested loops to iterate through numbers between low and high. Within the loops, for each number: Check if it's divisible by any number between 2 and itself (j).

# STEP 4 :
Run the java code to print the prime numbers N.

# PROGRAM :
```
<html>
<head>
<script type="text/javascript">
function show()
{
var low=Number(document.getElementById("n1").value);
var high=Number(document.getElementById("n2").value);
var i,j;
for(i=low;i<=high;i++) 
{
var flag=0;
for(j=2;j<i;j++) 
{
if(i%j==0) 
{
flag=1;
break;
}
}
if(flag==0&&i>1) 
alert(i);
}
}
</script>
</head>
<body>
<form>
<input type="text" id="n1">
<input type="text" id="n2">
<input type="button" onclick="show()" value="Generate">
</form>
</body>
</html>
```
# OUTPUT :
![image](https://github.com/Jeshwanthkumarpayyavula/ODD23-24-WT-JavaScript/assets/145742402/b7c7af3b-de9f-4ac4-b5b2-2eed77adb418)

# RESULT :
Thus the java code to print the prime numbers N has been executed successfully.

# QUESTION 04 :
# AIM :
To construct a JavaScript program to implement a simple calculator.

# PROCEDURE :
# STEP 1 :
Start with the basic 'html' structure. In the 'head', embed a 'script' tag to contain the JavaScript functions.

# STEP 2 :
Within the 'body', create a 'form' element for user interactions. Add multiple buttons, each representing a specific operation (e.g., Add, Subtract, Multiply, etc.). Include two input fields (input type="text") for users to input two numbers (n1 and n2). Provide an input field to display the result (n3).

# STEP 3 :
Define individual JavaScript functions (f1() to f9()) for each operation:

Addition (f1()): Add numbers a and b, then display the result in n3. Subtraction (f2()): Subtract b from a, then display the result. Multiplication (f3()): Multiply a and b, then display the result. Division (f4()): Divide a by b, then display the result. Sine (f5()): Calculate sine of a and display. Cosine (f6()): Calculate cosine of a and display. Tangent (f7()): Calculate tangent of a and display. Square (f8()): Square a and display the result. Clear (f9()): Clear all input and output fields.

# STEP 4 :
Run the code.

# PROGRAM :
```
<html>
<head>
<script type="text/javascript">
function f1()
{
var a=Number(document.getElementById("n1").value);
var b=Number(document.getElementById("n2").value);
document.getElementById("n3").value=a+b;
}
function f2()
{
var a=Number(document.getElementById("n1").value);
var b=Number(document.getElementById("n2").value);
document.getElementById("n3").value=a-b;
}
function f3()
{
var a=Number(document.getElementById("n1").value);
var b=Number(document.getElementById("n2").value);
document.getElementById("n3").value=a*b;
}
function f4()
{
var a=Number(document.getElementById("n1").value);
var b=Number(document.getElementById("n2").value);
document.getElementById("n3").value=a/b;
}
function f5()
{
var a=Number(document.getElementById("n1").value);
var b=Number(document.getElementById("n2").value);
document.getElementById("n3").value=Math.sin(a);
}
function f6()
{
var a=Number(document.getElementById("n1").value);
var b=Number(document.getElementById("n2").value);
document.getElementById("n3").value=Math.cos(a);
}
function f7()
{
var a=Number(document.getElementById("n1").value);
var b=Number(document.getElementById("n2").value);
document.getElementById("n3").value=Math.tan(a);
}


function f8()
{
var a=Number(document.getElementById("n1").value);
var b=Number(document.getElementById("n2").value);
document.getElementById("n3").value=a*a;
}
function f9()
{
document.getElementById("n1").value=" ";
document.getElementById("n2").value=" ";
document.getElementById("n3").value=" ";
}
</script>
</head>
<body>
<form>
<input type="button" onclick="f1()"  value="Add">
<input type="button" onclick="f2()"  value="Subtract">
<input type="button" onclick="f3()"  value="Multiply">
<input type="button" onclick="f4()"  value="Divide">
<input type="button" onclick="f5()"  value="Sin A">
<input type="button" onclick="f6()"  value="Cos A">
<input type="button" onclick="f7()"  value="Tan A">
<input type="button" onclick="f8()"  value="A Square">
<input type="button" onclick="f9()"  value="Clear">
<input type="text" id="n1">
<input type="text" id="n2">
<input type="text" id="n3">
</form>
</body>
</html>
```
# OUTPUT :
![image](https://github.com/Jeshwanthkumarpayyavula/ODD23-24-WT-JavaScript/assets/145742402/b699798b-baf7-4e84-a903-4b6a24decb57)

# RESULT :
Thus the java code for constructing a simple calculator has been executed successfully.

# QUESTION 05 :
# AIM :
To Design a simple text editor JavaScript application where we can manipulate the user input in different styles, edit the input, capitalize, and many string operations.

# PROCEDURE :
# STEP 1 :
Create an HTML file that will act as the foundation for our text editor. Inside the 'head' section, link to a JavaScript file.

# STEP 2 :
Define the Javascript functions like text bold, text italic, all uppercase, all lowercase etc.

# STEP 3 :
Add buttons in the form of input elements. Each button will have a specific action, like making text bold, aligning text, etc.

# STEP 4 :
Inside each JavaScript function, use the getElementById method to select the text area by its ID ("num"). Apply different styles to the text inside the text area based on the button clicked. For example, the fontWeight property changes the text to bold when the "Bold" button is clicked.

# STEP 5 :
Run the code and display the output.

# PROGRAM :
```
<html>
<head>
<script type="text/javascript">
function f1()
{
document.getElementById("num").style.fontWeight="bold";
}
function f2()
{
document.getElementById("num").style.fontStyle="italic";
}
function f3()
{
document.getElementById("num").style.textTransform="uppercase";
}
function f4()
{
document.getElementById("num").style.textTransform="lowercase";
}
function f5()
{
document.getElementById("num").style.textTransform="capitalize";
}
function f6()
{
document.getElementById("num").style.textAlign="right";
}
function f7()
{
document.getElementById("num").style.textAlign="left";
}
function f8()
{
document.getElementById("num").style.textAlign="center";
}



function f9()
{
document.getElementById("num").style.fontWeight = "normal";
document.getElementById("num").style.textAlign = "left";
document.getElementById("num").style.fontStyle = "normal";
}
</script>
</head>
<body>
<form>
<input type="button" onclick="f1()"  value="Bold">
<input type="button" onclick="f2()"  value="Italics">
<input type="button" onclick="f3()"  value="All Caps">
<input type="button" onclick="f4()"  value="Small Caps">
<input type="button" onclick="f5()"  value="Title Case">
<input type="button" onclick="f6()"  value="Align Right">
<input type="button" onclick="f7()"  value="Align Left">
<input type="button" onclick="f8()"  value="Align Center">
<input type="button" onclick="f9()"  value="Clear Formatting">
<textarea rows="10" cols="35" id="num">
Simple Text Editor using JavaScript
</textarea>
</form>
</body>
</html>
```
# OUTPUT :
![image](https://github.com/Jeshwanthkumarpayyavula/ODD23-24-WT-JavaScript/assets/145742402/089a572d-42cf-46d9-b9ad-6fe67b4d5e82)

# RESULT :
Thus the java code to design a simple text editor JavaScript application where we can manipulate the user input in different styles, edit the input, capitalize, and many string operations has been executed successfully.

# QUESTION 06 :
# AIM :
To Design a JavaScript program which displays error messages when a field in form is entered incorrectly.

# PROCEDURE :
# STEP 1 :
Create an HTML file and Create arrays for error divs and input values.

# STEP 2 :
Use validate() to check username, password, and confirmation inputs. Display errors or "OK!" messages accordingly.

# STEP 3 :
Inside validate(), compare password and confirmation to ensure they match.

# STEP 4 :
Implement finalValidate() to ensure both username and password validations are correct before displaying a success message.

# STEP 5 :
Run the code and finally display the output.

# PROGRAM :
```
<html>
<head>
  <title>Form Validation</title>
  <script type="text/javascript">
    var divs = new Array();
    divs[0] = "errUserName";
    divs[1] = "errPassword";
    divs[2] = "errConfirm";
    function validate()
	{
      var inputs = new Array();
      inputs[0] = document.getElementById('username').value;
      inputs[1] = document.getElementById('password').value;
      inputs[2] = document.getElementById('confirm').value;
      var errors = new Array();
      errors[0] = "<span style='color:red'>Please enter your Username!</span>";
      errors[1] = "<span style='color:red'>Please enter your password!</span>";
      errors[2] = "<span style='color:red'>Please confirm your password!</span>";
      for (i in inputs)
      {
        var errMessage = errors[i];
        var div = divs[i];
        if (inputs[i] == "")
        	document.getElementById(div).innerHTML = errMessage;
        else if (i==1)
        {
          var first = document.getElementById('password').value;
          var second = document.getElementById('confirm').value;
          if (second != first)
        	document.getElementById('errConfirm').innerHTML = "<span style='color: red'>Your passwords don't match!</span>";
          else
       		document.getElementById(div).innerHTML = "OK!";
        }
        else
        	document.getElementById(div).innerHTML = "OK!";
       }
     }
        function finalValidate()
        {
          var count = 0;
          for(i=0;i<2;i++)
          {
            var div = divs[i];
            if(document.getElementById(div).innerHTML == "OK!")
            count = count + 1;
          }
          if(count == 2)
          	document.getElementById("errFinal").innerHTML = "All the data you entered is correct!!!";
        }
   </script>
</head>
<body>
	<table id="table1">
      <tr>
        <td>User Name:</td>
        <td><input type="text" id="first" onkeyup="validate();" /></td>
        <td><div id="errUserName"></div></td>
      </tr>
      <tr>
        <td>Password:</td>
        <td><input type="password" id="password" onkeyup="validate();"/></td>
        <td><div id="errPassword"></div></td>
      </tr>
      <tr>
        <td>Confirm Password:</td>
        <td><input type="password" id="confirm" onkeyup="validate();"/></td>
        <td><div id="errConfirm"></div></td>
      </tr>
      <tr>
        <td><input type="button" id="create" value="Create" onclick="validate();finalValidate();"/></td>
        <td><div id="errFinal"></div></td>
      </tr>
	</table>
</body>
</html>
```
# OUTPUT :
![image](https://github.com/Jeshwanthkumarpayyavula/ODD23-24-WT-JavaScript/assets/145742402/637cf6ef-397b-4203-affb-514757d9d352)

# RESULT :
Thus the java code to Design a JavaScript program which displays error messages when a field in form is entered incorrectly has been executed successfully.

