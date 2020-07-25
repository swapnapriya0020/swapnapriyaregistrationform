<!DOCTYPE html>
<html lang="en">
<head>
    <script>
function validateForm() {
  var x = document.forms["myForm"]["phone"].value;
  if (x == " ") {
    alert("phone must be filled out");
    return false;
  }
}
</script>
</head>
  <title>Registration form</title>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
</head>
<body>
<div class="login-form">
  <form name="myForm" onsubmit="return validateForm()" method="post">
    <button type="submit" class="btn">Sign In</button>
    <div class="input-container">  
    <input class="input-field" type="text" placeholder="name@gmail.com" name="email" required>
    <i class="fa fa-envelope icon"></i>
</div>
<div class="input-container"> 
    <input type="password" placeholder="password" name="psw" required>
     <i class="fa fa-lock icon"></i>
 </div>
 <input type="number" name="phone" placeholder="mobile number">
    <button type="submit">SIGN IN</button>   
    <label class="forget-psw">Forgot your password? <a href="#"></a></label>
    <span>Register!</span>

    <div class="social-btn">
      
      <button type="submit" class="facebook-btn"><i class="fa fa-facebook" aria-hidden="true"></i></button>
      <button type="submit" class="google-btn"><i class="fa fa-google" aria-hidden="true"></i></button>
      <button type="submit" class="epam-btn"><i class="fa fa-epam" aria-hidden="true"><b>EPAM LOGIN</b></i></button>
    </div>
  </form>
</div>

<style type="text/css">
body {
    background-color: #fbfbfb;
}
.login-form {
    font-family: arial;
    color: #333;
} 
.login-form form {
    width: 500px;
    margin: 0 auto;
    padding: 20px 30px 20px;
    border: 1px solid #ddd;
    border-radius: 5px;
    box-sizing: border-box;
    background-color: #ffffff;
}
.login-form h2 {
    text-align: center;
    font-size: 35px;
    margin: 10px 0px 40px;
}
.login-form input {
    width: 100%;
    border: 1px solid #ddd;
    padding: 5px 10px;
    height: 45px;
    margin: 0px 0px 20px;
    border-radius: 4px;
    box-sizing: border-box;
    font-size: 17px;
}
.login-form button {
    margin: 10px auto 30px;
    display: table;
    font-size: 20px;
    padding: 10px 30px;
    background-color: lightseagreen;
    border: none;
    color: #fff;
    border-radius: 4px;
    cursor: pointer;
}

.input-container {
  display: -ms-flexbox; /* IE10 */
  display: flex;
  color:white;
  width: 100%;
  margin-bottom: 15px;
}
.icon {
  padding: 10px;
  background: white;
  color: grey;
  min-width: 50px;
  text-align: center;
}
.btn {
  background-color: dodgerblue;
  color: white;
  padding: 15px 20px;
  border: none;
  cursor: pointer;
  width: 100%;
  opacity: 0.9;
}

.btn:hover {
  opacity: 1;
}
.login-form button:hover{
  opacity: 0.8;
}
.login-form input[type="checkbox"] {
    height: 16px;
    width: 16px;
    margin-right: 5px;
    float: left;
}
.login-form .forget-psw {
    float: right;
}
.login-form .forget-psw a {
    color: #2196F3;
    text-decoration: none;
}
.social-btn button.google-btn, .social-btn button.facebook-btn, .social-btn button.epam-btn  {
    width: 100%;
    font-size: 18px;
    margin: 0px 0px 10px;
}
.social-btn button.google-btn{
  background-color: tomato;
}
.social-btn button.facebook-btn{
  background-color: #3f68be;
}
.social-btn button.epam-btn{
  background-color: greenyellow;
}
.social-btn {
    border-top: 1px solid #ddd;
    padding-top: 30px;
    margin-top: 30px;
}
.bttn{
    border-top: 1px solid greenyellow;
    padding-top: 30px;
    margin-top: 30px;
}
.social-btn button i {
    margin-right: 5px;
    font-size: 20px;
}
@media (max-width: 767px){
.login-form form {
    width: 90%;
    padding: 20px 15px 20px;
}
.social-btn button.google-btn, .social-btn button.facebook-btn {
    font-size: 15px;
}
} 
</style>

</body>
</html>
