<!DOCTYPE html>
<html>
  <head>
    <base target="_top">
    
  </head>
  <style>
  
  *{
  letter-spacing:.01em;
  color:navy;
  }
  
  body{
  background:#FFFFCF   url("https://tdm.usinternet.com/customers/order/assets/img/icons/edit.png") no-repeat 80% 50%;
  }
  
  #one{
  border: 5px double brown;
  border-radius: 5px;
  outline-style: solid;
  }
  .button {
    background-color: #ff8000;
    border: none;
    color: white;
    padding: 9px 15px;
    text-align: center;
    text-decoration: none;
    display: inline-block;
    font-size: 16px;
    margin: 4px 2px;
    cursor: pointer;
}
.button:hover { 
    box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
}  
  
  
  
  </style>
  <body bgcolor="BlanchedAlmond" >
<script src="registration.js"></script>


<div id="one">
<h4 align="center"style="padding: .01px 10px .01px 10px;letter-spacing:.2px; border-style:outset; border-color:brown;"><b><u>Enter Details For Registration</u></b></h4><br>
<div style="margin-left:40px;">
<form name="form1" action="" method="post" onreset="myFunction()" onsubmit="getConfirmation()">

    <div style="color:red" id="errorname"></div>
    Name:<input type="text" name="name" id="name" onblur="validateName()" placeholder="Full name" style="margin-left:20px; "/><br>
    
    <div style="color:red" id="errordob" ></div>
    DOB:<input type="date" name="dob" id="dob"  onblur="validatedob()"  size="30" style="margin-left:24px; width:168px; "/><br>
    
    <div style="color:red" id="errorage" ></div>
    Age:<input type="text" name="age" maxlength="2" id="age" onclick="agefinding()" onblur="validateAge()" placeholder="5<Age of the member<70" style="margin-left:31px;" readonly/><br>
     
    <div style="color:red" id="errorgender" ></div>
    Gender:<select name="gender"  id="gender" onchange="validateGender()" style="margin-left:10px; width: 172px;">
        <option value="select">select</option>
        <option value="Male">Male</option>
        <option value="Female">Female</option>
    </select><br>
   
    <div style="color:red" id="errorcontact" ></div>
    Contact:<input type="text" name="no" maxlength="10"  id="no" onblur="validateContact()" placeholder="Enter number" style="margin-left:8px;"/><br>
    
    <div style="color:red" id="erroraddr" ></div>
    Address:<input type="text" name="addr" id="addr" placeholder="Present Address" onblur="validateAddr()" style="margin-left:5px;"/><br>
    
    <div style="color:red" id="errorinterest" ></div>
    Interest:&nbsp;<select name="interest" id="interest" onchange="validateinterest()" style="margin-left:5px;width: 173px;" >
        <option value="select">select</option>
        <option value="Gymm">Gymm</option>
        <option value="Yoga">Yoga</option>
    </select><br>
    
        <label for="msg"  >Suggestion:</label><br>
        <textarea id="msg" name="msg" id="msg"></textarea><br><br>
    
    <input type="reset" class="button" style="color:white;">
<input type="submit" class="button" name="Register" value="Register" style="color:white;" onclick="return validationForm()"/>
<br><br><br>
</form>    
</div>
</div>
  </body>
</html>


