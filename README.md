# TEAM1_Comp231
Customer Registration form

Team #1, Comp 231, Project, Customer Registration Form and Payment via paypal

<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">

<head>
<meta content="text/html; charset=utf-8" http-equiv="Content-Type" />
<title>Comp 231 Team 1 Project</title>
<link rel="stylesheet" type="text/css" href="validateForm.css"/> 
<style type="text/css">
.div1{
	margin:auto;width:50%;border:3px solid green;padding:10px;
	margin-top:50px;background-color:silver;
	margin-bottom:100px;
	margin-right:50px;
	margin-left:200px
   }
   .div2{
	margin:auto;width:73%;border:3px solid black;padding:10px;
	margin-top:5px;background-color:silver;
	margin-bottom:50px;
	margin-right:50px;
	margin-left:80px
   }
   .div3{
	margin:auto;width:73%;border:3px solid black;padding:10px; 
	margin-top:5px;background-color:silver;
	margin-bottom:50px;
	margin-right:50px;
	margin-left:80px
   }
   .div4{
	margin:auto;width:73%;border:3px solid black;padding:10px; 
	margin-top:5px;background-color:silver;
	margin-bottom:50px;
	margin-right:50px;
	margin-left:80px
   }

.div5{
	margin:auto;width:73%;border:3px solid black;padding:10px; 
	margin-top:5px;background-color:silver;
	margin-bottom:50px;
	margin-right:50px;
	margin-left:80px
   }
.redReq {
	color: #FF0000;
}
.auto-style1 {
	margin-right: 0px;
}
</style>

</head>
<script type="text/javascript" src="validateForm.js"></script>
<body>
<div class="div1">
<p align="center" style="color:green">GYM REGISTRATION FORM</p>
<form action="/action_page.php" method="post">

<fieldset>
<legend>Personal Information</legend>
<div class="div2">
<table>
<tr>
<td>
First Name<span class="redReq">*</span><br/>
<input type="text" name="fname" id="firstName" placeholder="Please enter your first name" size="30" maxlength="100"/>
</td>
<td>
Last Name<span class="redReq">*</span><br/>
<input type="text" name="lname" id="lastName" placeholder="Please enter your last name" size="30"maxlength="100"/>
</td>
</tr>
<tr>
<td>
Gender<span class="redReq">*</span><br/>
<input type="text" name="gender" id="genderType" placeholder="Please put your Gender" size="30" maxlength="6"/>
</td>
</tr>
<tr>
<td>
Other(Please specify)<br/>
<input type="text" name="otherInputType" placeholder="Please specify others if you have any" size="30"maxlength="100"/>
</td>
</tr>
</table>
  </div>
</fieldset>

<fieldset>
<legend>Contact Information</legend>
<div class="div3">
<table>
<tr>
<td style="width: 378px">
Street Address<span class="redReq">*</span><br/>
<input type="text" name="streetAddress" id="streetAddress" placeholder="Please enter your Street Address" size="30" maxlength="100" style="width: 486px"/>
</td>
</tr>
</table>
<table class="auto-style1" style="width: 409px">
<tr>
<td>
City<span class="redReq">*</span><br/>
<input type="text" name="cityName" id="cityName" placeholder="Please enter the City Name" size="30"maxlength="100"/>
</td>
<td>
Province<span class="redReq">*</span><br/>

<input type="text" name="province" id="provinceName" placeholder="Please enter the name of the province" style="width: 238px"/> 
</td>
</tr>
<tr>
<td>
Postal Code<span class="redReq">*</span><br/>
<input type="text" name="postalCodeForm" id="postalCode" placeholder="Postal Code [A1A 2B2]" size="30"maxlength="100"/>
</td>
<td>
Country<span class="redReq">*</span><br/>
<input type="text" name="countryName" id="countryName" placeholder="Please enter your country" size="30"maxlength="100" style="width: 238px"/>
</td>
</tr>
<tr>
<td>Phone<span class="redReq">*</span><br/>
<input type="text" name="phone" id="phone" placeholder="416-999-1234" size="30"maxlength="100"/>
</td>
<td>E-mail<span class="redReq">*</span><br/>
<input type="text" name="email" id="email" placeholder="yourEmail@email.com" size="30"maxlength="100"/>
</td>
</tr>
</table>
</div>
</fieldset>

<fieldset>
<legend>Login Information</legend>
<div class="div4">
<table>
<tr>
<td>
User Name<span class="redReq">*</span><br/>
<input type="text" name="userName" id="userName" placeholder="Please enter your user Name" size="30" maxlength="100"/>
</td>
</tr>
<tr>
<td>
Password<span class="redReq">*</span><br/>
<input type="text" name="userPassword" id="userPassword" placeholder="Please enter your password" size="30"maxlength="100"/>
</td></tr>
<tr><td>
Confirm Password<span class="redReq">*</span><br/>
<input type="text" name="userConfirmPassword" id="confirmPassword" placeholder="Please re-renter your password" size="30"maxlength="100"/>
</td>
</tr>
</table>
</div>
</fieldset>

<fieldset>
<legend>Membership Information</legend>
<div class="div5">
<table>
<tr>

<td>
Program of Interest<span class="redReq">*</span><br/>
<select name="programOfInterest" id="programOfInterest" placeholder="name">
  <option value=""></option>
  <option value="Gold">Gold</option>
  <option value="Silver">Silver</option>
  <option value="Platinum">Platinum</option>
</select>
</td>
</tr>
<tr>
<td>
Prefered Trainer<span class="redReq">*</span><br/>
<input type="text" name="preferredTrainer" id="PreferredTrainer" placeholder="name" size="30" maxlength="100"/>
</td>
</tr>
<tr>
<td>
How did you hear about us?<br/>
<input type="text" name="reference" id="reference" placeholder="Website, Conference ie" size="30"maxlength="100"/>
</td>
</tr>
</table>
</div>
</fieldset>
<fieldset>
<legend>Payment</legend>
<div id="paypal-button-container"></div>
</fieldset>

</form>

<p><span class="redReq">*</span> Required Field</p>
<input type="submit" value="Submit" onclick="validateForm()"/>

</div>
<script>
function validateForm()
	{
		// ===========Returns the element that has the ID attribute with the specified value===========
    	var first_name = document.getElementById("firstName");	//First name
        var last_name = document.getElementById("lastName");	//Last name
        var gender = document.getElementById("genderType");	//Gender
        var street_address = document.getElementById("streetAddress");	//Street address
        var city_name = document.getElementById("cityName");	//City
        var postal_code = document.getElementById("postalCode");	//Postal code	
        var province_name = document.getElementById("provinceName");	//Province
        var password = document.getElementById("userPassword");	//Password (first field)					
        var confirm_password = document.getElementById("confirmPassword");	// Confirm password                
        var email_address = document.getElementById("email");	//Email address		  
        var user_name = document.getElementById("userName"); // login user name
        var country_name = document.getElementById("countryName");	//country name
        var phone_number = document.getElementById("phone");	// phone 
        var program_of_interest = document.getElementById("programOfInterest");	// program of interest
        var preferred_trainer = document.getElementById("PreferredTrainer");	// preferred trainer
        		
		//=============search pattern============================================
        var first_name_regex = "^[A-Z]{1,}[a-z]*";	//First name and Last name 
        var postal_code_regex = "[A-Za-z][0-9][A-Za-z] ?[0-9][A-Za-z][0-9]"; //postal code
        var phone_number_regex = "[0-9]{10}";	// phone number
        var email_address_regex = "[a-z0-9]+@[a-z0-9]+\.[a-z]{2,3}$";	// email address
        var password_regex = "^(?=.*?[a-z])(?=.*?[0-9])(?=.*?[./]).{8,12}$";	// password
        
		// Checking the first name field if its empty or not
        if (first_name.value.length == 0)
        	{
            	alert("Your First name can not be empty");
                return false;
            }
		// Checking the first name field character limit
        if (first_name.value.length < 15) 
        	{
        		alert("Your First Name MUST contain at least 15 characters or more");
                return false;
            }
        // searching the first name and checking the first character is upper case or not
        if (first_name.value.match(first_name_regex) == null) 
        	{
                alert("First character of your FIRST name MUST be a UPPER case");
                return false;
            }
        // Checking the last name field if its empty or not
        if (last_name.value.length == 0) 
        	{
            	alert("Your Last name can not be empty");
                return false;
            }
        // checking character limit of the last name field
        if (last_name.value.length < 15) 
        	{
                alert("Your Last Name MUST contain at least 15 characters or more");
                return false;
            }
        // searching the last name and checking the first character is upper case or not
        if (last_name.value.match(first_name_regex) == null) 
        	{
                alert("First character of your LAST name MUST be a UPPER case");
                return false;
            }
        // checking if gender field is empty or not
        if (gender.value.length == 0)
        	{
        		alert ("Please put your Gender");
        		return false;
        	}
        // checking if street address field is empty or not
         if (street_address.value.length == 0) 
          	{
                alert("Please enter your home address.");
                return false;
            }
        // checking the city field is empty or not
        if (city_name.value.length == 0) 
         	{
                alert("Please enter the city.");
                return false;
            }
        // checking the format for postal code
        if (postal_code.value.match(postal_code_regex) == null) 
            {
                alert("Postal code is in the wrong format. Please put a valid format: A9A 9A9");
                return false;
            }
        // checking the province field is empty or not 
        if (province_name.value.length == 0) 
         	{
                alert("Please enter the name of your province");
                return false;
            }
        // checking country name field
        if (country_name.value.length == 0)
        {
        	alert("Please enter the name of country");
        	return false;
        }
        // checking the phone number for 10 digits
        if (phone_number.value.match(phone_number_regex) == null)
        	{	
        		alert ("Please enter the right formar phone number. It has to be 10 digits");
        		return false;
        	}
       	// checking the format of the email address
        if (email_address.value.length == 0) 
            {
            	alert("Please enter your email address!");
                return false;
            }
        if (email_address.value.match(email_address_regex) == null) 
            {
                alert("Please verify your email address is in the correct order or not!!!");
                return false;
            }
         // checking login user name is empty or not
        if (user_name.value.length == 0)
        	{
        		alert("Your login name can not be empty");
        		return false;
        	}
        //checking user password fields
        if (password.value.length == 0) 
            {
            	alert("Please enter your password.");
                return false;
            }
        //verifying passowrd policy
        if (password.value.match(password_regex) == null) 
            {
            	alert("Password field length must be 8 to 12 characters and must include numbers, dot (.) and back slash (/).");
                return false;
            }
		// matching this field with password field
        if (password.value != confirm_password.value) 
            {
            	alert("password and confirm password do not match");
                return false;
            }              
     			//checking user program of interest fields
        if (program_of_interest.value.length == 0) 
            {
            	alert("Please enter your preferred area");
               return false;
            }
		//checking user preferred campus fields
        if (preferred_trainer.value.length == 0) 
            {
            	alert("Please enter your Preferred trainer name");
                return false;
            }
		
    	alert("You have successfully submitted your information, we will assess and get back to you soon");
	}
</script>
<script src="checkout.js"></script>



<script>

    // Render the PayPal button

    paypal.Button.render({

        // Set your environment

        env: 'sandbox', // sandbox | production

        // Specify the style of the button

        style: {
            label: 'pay',
            size:  'small', // small | medium | large | responsive
            shape: 'rect',   // pill | rect
            color: 'gold'   // gold | blue | silver | black
        },

        // PayPal Client IDs - replace with your own
        // Create a PayPal app: https://developer.paypal.com/developer/applications/create

        client: {
            sandbox:    'AZDxjDScFpQtjWTOUtWKbyN_bDt4OgqaF4eYXlewfBP4-8aqX3PiV8e1GWU6liB2CUXlkA59kJXE7M6R',
            production: '<insert production client id>'
        },

        // Wait for the PayPal button to be clicked

        payment: function(data, actions) {
            return actions.payment.create({
                payment: {
                    transactions: [
                        {
                            amount: { total: '0.01', currency: 'USD' }
                        }
                    ]
                }
            });
        },

        // Wait for the payment to be authorized by the customer

        onAuthorize: function(data, actions) {
            return actions.payment.execute().then(function() {
                window.alert('Payment Complete!');
            });
        }
 }, '#paypal-button-container');

</script>
</body>
</html>
