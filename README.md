# RowleySanchezm.github.io
<!DOCTYPE html> 

<html> 

<head> 

<style> 

body, input { font-family: Arial, Helvetica, "sans-serif"; font-size: 15px; } 

</style> 





<script> 



function validate() { 

	var x = document.forms["Form"]["Name"]; 
	var y = document.forms["Form"]["Email"]; 

		if (x.value == "") { 
		x.style.borderColor = "red"; 
		alert("Name must be filled out"); 
		return false; 

	} 
	else if (y.value == “”){
		y.style.borderColor = “red”;
		alert(“Email must be filled out”);
		return false;

	} 
	else if (y.value !== “” || x.value !==“”){
		x.style.borderColor = “black”;
		y.style.borderColour = “black”;
	}
}

</script> 

</head> 

<body> 



<form name="Form" onsubmit="return validate()"> 

Name: <input type="text" name="Name"><br> 

Email: <input type ="text" name="Email"> 

<input type="submit" value="Submit"> 



</form> 



</body> 

</html>
