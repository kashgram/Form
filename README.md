# Form
Login or Register?
<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <title>Button</title>
  </head>
  <link rel="stylesheet" href="style1.css">
  <body>
  <div class="hero">
    <div class="form-box">
<div class="button-box">
  <div id="btn">
  </div>
  <button type="button" class="toggle-btn" onclick="login()">Log In</button>
  <button type="button" class="toggle-btn" onclick="register()">Register</button>
</div>
<div class="smedia">
  <img src="fb.jpg">
  <img src="tw.jpg">
  <img src="gp.jpg">
</div>
<form id="login" class="input-group">
  <input type="text" class="input-field" placeholder="User ID" required>
  <input type="password" class="input-field" placeholder="Enter Password" required>
  <input type="checkbox" class="checkbox"><span>Remember Password.</span>
  <button type="submit" class="submit-btn">Log In</button>
</form>
<form id="register"class="input-group">
  <input type="text" class="input-field" placeholder="User ID" required>
  <input type="email" class="input-field" placeholder="Email ID" required>
  <input type="password" class="input-field" placeholder="Enter Password" required>
  <input type="checkbox" class="checkbox"><span>I Agree to the Terms & Conditions.</span>
  <button type="submit" class="submit-btn">Register</button>
</form>

    </div>
      </div>
      <script>
        var x = document.getElementById("login")
        var y = document.getElementById("register")
        var z = document.getElementById("btn")

        function register(){
          x.style.left="-400px"
          y.style.left="50px"
          z.style.left="110px"
         }
         function login(){
           x.style.left="50px"
           y.style.left="450px"
           z.style.left="0px"
          }
        </script>
  </body>
</html>
*{
  margin: 0 ;
  padding: 0;
  font-family: sans-serif;
}
.hero{
height: 100%;
width: 100%;
background-image:url(banner.jpg);
background-position:center;
background-size: cover;
position: absolute;
}
.form-box{
width: 380px;
height:480px;
position: relative;
margin: 6% auto;
background: #fff;
padding: 5px;
overflow: hidden;
}
.button-box{
  width: 220px;
  margin: 35px auto;
  position: relative;
  box-shadow: 0 0 20px 9px #ff61241f;
  border-radius: 30px;
}
.toggle-btn{
padding:10px 30px;
cursor: pointer;
background: transparent;
border: 0;
outline: none;
position: relative;
}
#btn{
  top: 0;
  left: 0;
  position: absolute;
  width: 110px;
  height: 100%;
  background: linear-gradient(to right,#ff105f,#ffad06);
  border-radius: 30px;
  transition: 0.5s;
}
.smedia{
  margin: 30px auto;
  text-align: center;
}
.smedia img{
  width: 30px;
  margin: 0 12px;
  box-shadow: 0 0 20px 0 #7f7f7f3d;
  cursor: pointer;
  border-radius: 50%;
}
.input-group{
top: 180px;
position: absolute;
width: 288px;
transition: .5s;
}
.input-field{
  width: 100%;
  padding: 10px 0px;
  margin: 5px 0px;
  border-top: 0;
  border-bottom: 1px solid #999;
  border-left: 0;
  border-right: 0;
  outline: none;
  background: transparent;
}
.submit-btn{
  width: 85%;
  padding: 10px 30px;
  cursor: pointer;
  display: block;
  margin: auto;
  background: linear-gradient(to right,#ff105f,#ffad06);
  border: 0;
  outline: none;
  border-radius: 30px;
}
.checkbox{
  margin:30px 18px 30px 0;
}
span{
  color: #777;
  font-size: 12px;
  bottom: 68px;
  position: absolute;
}
#login{
  left: 50px;
}
#register{
  left: 450px;
}
