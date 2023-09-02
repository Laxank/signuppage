<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        body{
            overflow: hidden;
            background: linear-gradient(rgb(250, 134, 153) ,rgb(45, 157, 255))
     
           
        }

    .log{
       

      border: 2px solid rgb(255, 255, 255);
        
      box-shadow: 0 0 20px 0 rgba(0,0,0,0.1);
      border-radius: 30px;
      background-color: white;
      background-position: center;
      align-items: center;
        width: 30%;
        height: 85vh;
        margin-top: 25%;
        margin-left: 50%;
        transform: translate(-50%, -50%);
    }
    .title{
        text-align: center;
        margin: 50px 200px;
     font-family: Arial, Helvetica, sans-serif;
     font-size: small;
      line-height: 50px;
        border-radius: 60px;
        border: snow;
        box-shadow: 0 0 20px 0 rgba(0,0,0,0.1);

    }
    
    .log form{
        padding: 0 40px;
        box-sizing: border-box;
    }
    form .text_fild{
        margin-top: 50px;
       position: relative;
     border-bottom: 2px solid silver;
       margin: 30px 0;
       

    }
    .text_fild input{
        width: 100%;
   padding: 0 -5px;
        height: 40px;
        font-size: 17px;
        background: none;
      border: none;
      outline: none;
      font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
        
    }
    .text_fild label{
        position: absolute;
        left: 35px;
        top: 50%;
        transform: translate(-50%);
        pointer-events: none;
        color: silver;
        font-size: 17px;
        transition: 0.5s;
    }
    .l label{
        position: absolute;
        left: 65px;
        top: 50%;
        transform: translate(-50%);
        pointer-events: none;
        color: silver;
        font-size: 17px;
        transition: 0.5s;
    }
    .text_fild span::before{
        content: '';
        position: absolute;
        top: 42px;
        height: 2px;
        left: 0;
        width: 0;
    
     
    }
    
    .text_fild input:focus~label ,.text_fild input:valid~label{
        top: -15px;
        color: rgb(0, 0, 0);
        font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;

    }
    .text_fild input:focus~.l label ,.text_fild input:valid~.l label{
        top: -15px;
        color: rgb(0, 0, 0);
        font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;

    }
    .text_fild input:focus~span::before ,.text_fild input:valid~span::before{
       width: 100%;
   background-color: blueviolet;
  

    }
    
    input[type="submit"]{
        width: 100%;
    
        height: 5vh;
        background-color: blueviolet;
        border-radius: 10px;
        font-size: large;
        border: none;
        color: white;
        cursor: pointer;

    
    }
    input[type="submit"]:hover{
      background-color: rgb(81, 22, 136);
    }
    .signup{
        font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
        text-align: center;
        margin-top: 30px;
    }
    input[type="checkbox"]{
        margin-bottom: 30px;
        position: relative;
    }
.line{
  
    position: relative;
    text-align: center;
    margin-top: 50px;
 

}



.line h3::before{
    content: '';
        position: absolute;
        top: 50%;
        height: 2px;
        background-color: silver;
        left: 30px;
        width: 200px;
}

.line h3::after{
    content: '';
        position: absolute;
        top: 50%;
        height: 2px;
        background-color: silver;
        right: 30px;
        width: 200px;
}
.opction{
  
    text-align: center;
    margin: 20px 70px;
    border-radius:30px;
    border: snow;
   line-height: 30px;
    box-shadow: 0 0 20px 0 rgba(0,0,0,0.1);
    cursor: pointer;
}
.opction h3{
  position: absolute;
  margin-top: 15px;
  margin-left: 100px;
 

  
}

.dp1{
  margin-left: -220px;
  margin-top: 10px;
    width: 10%;
    height: 5vh;
  display: inline-block;
    border-radius: 60%;
    object-fit: cover;
}
.dp1 img{
    width: 100%;
    height: 5vh;
    align-items: center;
    background-position: center;
  display: inline-block;
    border-radius: 60%;
    object-fit: cover;
    transition: 0.5s;
    cursor: pointer;
}
.dp1 img:hover{
  transform: translateY(-10px);
}



    </style>
</head>
<body>
    
    <div class="log">
        <div class="title"><h1>Sign Up</h1></div>
      
       
        <form method="form">
           
            <div class="text_fild">
                <input type="text" required>
                <span></span>
                <label>Usarname</label>
            </div>
            <div class="text_fild">
                <input type="text" required>
                <span></span>
                <label>Password</label>
            </div>
            <div class="text_fild">
                <input type="text" required>
                <span></span>
                <div class="l">
                    <label>Confirm Password</label>
                </div>
                
            </div>
            <div>
                <input type="checkbox" value="remindar"> Remember me
            </div>
            
          
            <input type="submit" value="Sign Up">
            <div class="signup">
                Already have account <a href="login_page.html">Login</a>
            </div>

            <div class="line">
               
                <h3>or</h3>
               
            </div>
            <div class="opction">
                <h3>Sign up with in gooogle</h3>
             
                    <div class="dp1">
                        <img src="C:\Users\REYZEN\Downloads/2005.jpg" alt="" style="width: 100%;
                        height: 4.2vh;"> 
                   </div>
               
            </div>
            <div class="opction">
                <h3>Sign up with in facebook</h3>
                <div class="dp1">
                    <img src="C:\Users\REYZEN\Downloads/2008.png" alt="" style="width: 100%;height: 4vh;">
                </div>
            </div>
           
        </form>
        
    </div>
    
    
</body>
</html>


<!-- <div class="dp1">
    <img src="C:\Users\REYZEN\Downloads/2005.jpg" alt="" style="width: 80%;
    height: 4.2vh;"> 
</div> -->
