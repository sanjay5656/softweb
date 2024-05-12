# Ex.07 Software Product Company Website
## Date:12/05/2024

## AIM:
To develop a static company website to display the softwares and services provided by the company.

## DESIGN STEPS:

### Step 1:
Requirement collection.

### Step 2:
Creating the layout using HTML and CSS.

### Step 3:
Updating the sample content.

### Step 4:
Choose the appropriate style and color scheme.

### Step 5:
Validate the layout in various browsers.

### Step 6:
Validate the HTML code.

### Step 7:
Publish the website in the given URL.

## PROGRAM:
### HOME
```HTML
<html>
    <head>
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>SAN INDUSTRY</title>
        <link rel="stylesheet" href="a.css">
        <style type="text/css">
            .logo {
                color: #ffffff;
                font-size: 40px;
                font-weight: 700;
                letter-spacing: 3px;
            }
            form {
                width: 300px;
                height: 40px;
                display: flex;
                background: rgba(255, 255, 255, 0.2);
                padding: 1px 1px;
                font-size: 15px;
                border-radius: 10px;
                backdrop-filter: blur(4px) saturate(180%);
            }
            form input {
                background: transparent;
                flex: 1;
                border: 0;
                outline: none;
                padding: 12px 20px;
                font-size: 15px;
                color: white;
            } 
            form button {
                border: 0;
                outline: none;
                padding: 5px 20px;
                color: white;
                border-radius: 10px;
                background: #00d5ff;
                cursor: pointer;
            }
            .navbar li {
                list-style: none;
                display: inline-block;
                margin: 0 20px;
                position: relative;
            }
            .navbar li a {
                text-decoration: none;
                color: white;
                text-transform: uppercase;
            }
            .navbar li:hover {
                border: 1px;
                padding: 10px;
                color: white;
                background-color: #00d5ff;
                transition: 0.5s; 
                cursor: pointer;
                border-radius: 30px;
            }
            .content {
                position: absolute;
                top: 50%;
                left: 50%;
                transform: translate(-50%,-50%);
                text-align: center;
            }
            .text h2 {
                color: white;
                font-weight: 800;
                font-size: 50px;
                letter-spacing: 3px;
            }
            .text p {
                color: white;
                text-transform: capitalize;
                font-size: 15px;
                margin-bottom: 30px;
                word-spacing: 2px;
                letter-spacing: 1px;
            }
            .login {
                margin: 0px 10px;
                border: 2px solid #00d5ff;
                padding: 13px 35px;
                letter-spacing: 1px;
                color: white;
                border-radius: 30px;
                background-color: #00d5ff;
                text-decoration: none;
            }
            .login:hover {
                border: 2px solid #00d5ff;
                color:  #00d5ff;
                background-color: white;
                transition: 0.5s;
                cursor: pointer;
            } 
            .signup {
                margin: 0px 10px;
                border: 2px solid #00d5ff;
                padding: 13px 35px;
                letter-spacing: 1px;
                color: white;
                border-radius: 30px;
                background-color: #00d5ff;
                text-decoration: none;
            }
            .signup:hover {
                border: 2px solid #f60b0b;
                color: #00d5ff;
                background-color: white;
                transition: 0.5s;
                cursor: pointer;
            }
        </style>
    </head>
    <body style="background-color: #6eded5;">
    <div class="banner">
        <br>
        <div class="navbar">
            <h1 class="logo">SAN PRODUCTS</h1>
            <ul>
                <li><a href="home.html"> Home </a></li>
                <li><a href="product.html"> Products </a></li>
                <li><a href="people.html"> People </a></li>
                <li><a href="contact.html"> Contact </a></li>
            </ul>
        </div>
        <div class="content">
            <div class="text">
                <h2>We provide innovative software solutions and services to help businesses thrive.</h2>
                <br><br><br><br><br>
                <div>
                    <a href="#" class="login"> Log In </a>
                    <a href="#" class="signup"> Sign Up </a>
                </div>
            </div>
        </div>  
    </div>
    <footer>
        <center>Developed by SANJAY S (212221243002) </center>
    </footer>
</body>
</html>
```

### PRODUCT
```HTML
<html>
    <head>
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title> Product Page </title>
        <link rel="stylesheet" href="a.css">
        <style type="text/css">
            .logo {
                color:  #ffffff;
                font-size: 40px;
                font-weight: 700;
                letter-spacing: 3px;
            }
            form {
                width: 300px;
                height: 40px;
                display: flex;
                background: rgba(255,255, 255, 0.1);
                padding: 1px 1px;
                font-size: 15px;
                border-radius: 10px;
                backdrop-filter: blur(4px) saturate(180%);
            }
            form input {
                background: transparent;
                flex: 1;
                border: 0;
                outline: none;
                padding: 12px 20px;
                font-size: 15px;
                color: white;
            } 
            form button {
                border: 0;
                outline: none;
                padding: 5px 20px;
                color: white;
                border-radius: 10px;
                background:  #00d5ff;
                cursor: pointer;
            }
            .navbar li {
                list-style: none;
                display: inline-block;
                margin: 0 20px;
                position: relative;
            }
            .navbar li a {
                text-decoration: none;
                color: white;
                text-transform: uppercase;
            }
            .navbar li:hover {
                border: 1px;
                padding: 10px;
                color: white;
                background-color:  #00d5ff;
                transition: 0.5s; 
                cursor: pointer;
                border-radius: 30px;
            }
            .container {
                background: transparent;
                padding: 10px 5%;
                padding-bottom: 100px;
            }
            .container .box-container {
                display: grid;
                grid-template-columns: repeat(auto-fit, minmax(170px, 1fr));
                gap: 100px;
            }
            .container .box-container .box {
                color: white;
                box-shadow: 0 5px 10px rgba(0,0,0,.2);
                border-radius: 20px;
                background: transparent;
                border: 1px solid white;
                padding: 30px 20px;
            }
            .container .box-container .box img {
                height: 70px;
                border-radius: 20px;
            }
            .container .box-container .box h3 {
                color:  #00d5ff;
                font-size: large;
                padding: 20px 0;
            }
            .container .box-container .box p {
                color: white;
                font-size: small;
                line-height: 1.5;
            }
        </style>
    </head>
<body style="background-color: #6eded5;">
    <div class="banner">
        <br>
        <div class="navbar">
            <h1 class="logo">SAN PRODUCTS</h1>
            <ul>
                <li><a href="home.html"> Home </a></li>
                <li><a href="product.html"> Products </a></li>
                <li><a href="people.html"> People </a></li>
                <li><a href="contact.html"> Contact </a></li>
            </ul>
        </div>
        <div class="container">
            <div class="box-container">
                <div class="box">
                    <img src="C:\Users\Sanjay S\softweb\1.jpg" alt="">
                    <h3> Web development </h3>
                    <p> Web development company helps you build a website or an application for business or personal use. </p>
                </div>
                <div class="box">
                    <img src="C:\Users\Sanjay S\softweb\2.jpg" alt="">
                    <h3> Software development </h3>
                    <p> Design, develop and maintain applications, frameworks or other software components for businesses or consumers. </p>
                </div>
                <div class="box">
                    <img src="C:\Users\Sanjay S\softweb\3.png" alt="">
                    <h3> AI software</h3>
                    <p> protect your systems, data, and networks with algorithms and robust AI - ML approaches.  </p>
                </div>
                <div class="box">
                    <img src="C:\Users\Sanjay S\softweb\4.jpeg" alt="" width="130px">
                    <h3> Android app development </h3>
                    <p> Android development is the process of creating applications for devices running an Android operating system.  </p>
                </div>
                <div class="box">
                    <img src="C:\Users\Sanjay S\softweb\5.jpeg" alt="">
                    <h3> Apple app development </h3>
                    <p> The process of creating software applications that run on a mobile device. </p>
                </div>
            </div>
        </div>
    </div>
    <footer>
        <center>Developed by SANJAY S (212221243002) </center>
    </footer>
</body>
</html>
```

### PEOPLE
```HTML
<html>
    <head>
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title> people page </title>
        <link rel="stylesheet" href="a.css">
        <style type="text/css">
            .logo {
                color: #ffffff;
                font-size: 40px;
                font-weight: 700;
                letter-spacing: 3px;
            }
            form {
                width: 300px;
                height: 40px;
                display: flex;
                background: rgb(102, 29, 29);
                padding: 1px 1px;
                font-size: 15px;
                border-radius: 10px;
                backdrop-filter: blur(4px) saturate(180%);
            }
            form input {
                background: transparent;
                flex: 1;
                border: 0;
                outline: none;
                padding: 12px 20px;
                font-size: 15px;
                color: white;
            }
            form button {
                border: 0;
                outline: none;
                padding: 5px 20px;
                color: white;
                border-radius: 10px;
                background: #00d5ff;
                cursor: pointer;
            }
            .navbar li {
                list-style: none;
                display: inline-block;
                margin: 0 20px;
                position: relative;
            }
            .navbar li a {
                text-decoration: none;
                color: white;
                text-transform: uppercase;
            }
            .navbar li:hover {
                border: 1px;
                padding: 10px;
                color: white;
                background-color: #00d5ff;
                transition: 0.5s; 
                cursor: pointer;
                border-radius: 30px;
            }
            .image {
                position: relative;
                border: 0;
                top: 150px;
                
                background: transparent;
            }
            .image table {
                border: 0;
                color: white;
                position: relative;
                left: 200px;
                
            }
            .image table img {
                height: 140px;
                width: 140px;
                border: 2px solid white;
                padding: 5px;
                border-radius: 50%;
            }
            .image table td {
                color: #00d5ff;
            }
        </style>
    </head>
<body style="background-color: #6eded5;">
    <div class="banner">
        <br>
        <div class="navbar">
            <h1 class="logo">SAN PRODUCTS</h1>
            <ul>
                <li><a href="home.html"> Home </a></li>
                <li><a href="product.html"> Products </a></li>
                <li><a href="people.html"> People </a></li>
                <li><a href="contact.html"> Contact </a></li>
            </ul>
        </div>
        <div class="image">
            <table cellspacing="20"> 
                <tr align="center">
                    <td> <img src="C:\Users\Sanjay S\softweb\vin.jpg"> </td>
                    <td> <img src="C:\Users\Sanjay S\softweb\paul_walker.jpg"> </td>
                    <td> <img src="C:\Users\Sanjay S\softweb\Jason Statham.jpg"> </td>
                    <td> <img src="C:\Users\Sanjay S\softweb\Jordana Brewster.jpg"> </td>
                    <td> <img src="C:\Users\Sanjay S\softweb\Tyrese Gibson.jpg"> </td>
                    <td> <img src="C:\Users\Sanjay S\softweb\Dwayne Johnson.jpeg"> </td>
                </tr>
                <tr align="center">
                    <th> VIN DIESEL</th>
                    <th> PAUL WALKER</th>
                    <th> JASON STATHAM</th>
                    <th> JORDANA BREWSTER </th>
                    <th> TYRESE GIBSON</th>
                    <th> DWAYRE JOHNSON</th>
                </tr>
                <tr align="center">
                    <td> CEO of AI</td>
                    <td> CEO of R7 </td>
                    <td> CEO of APPLE </td>
                    <td> Co-Founder R7  </td>
                    <td> CEO of ANDROID </td>
                    <td> CEO of ML </td>
                </tr>
            </table>
        </div>
    </div>
    <footer>
        <center>Developed by SANJAY S (212221243002) </center>
    </footer>
</body>
</html>
```

### CONTACT
```HTML
<html>
    <head>
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title> Contact Us Page </title>
        <link rel="stylesheet" href="a.css">
        <style type="text/css">
            .navbar form input {
                background: transparent;
                flex: 1;
                border: 0;
                outline: none;
                padding: 12px 20px;
                font-size: 15px;
                color: white;
            } 
            .navbar form button {
                border: 0;
                outline: none;
                padding: 5px 20px;
                color: white;
                border-radius: 10px;
                background: #00d5ff;
                cursor: pointer;
            }
            .navbar li {
                list-style: none;
                display: inline-block;
                margin: 0 20px;
                position: relative;
            }
            .navbar li a {
                text-decoration: none;
                color: white;
                text-transform: uppercase;
            }
            .navbar li:hover {
                border: 1px;
                padding: 10px;
                color: white;
                background-color: #00d5ff;
                transition: 0.5s; 
                cursor: pointer;
                border-radius: 30px;
            }
            .box {
                display: flex;
                column-gap: 40px;
                background: transparent;
                position: relative;
                top: 50px;
            }
            .box-1 {
                height: 400px;
                width: 400px;
                border: 3px solid white;
                border-radius: 20px;
                background: transparent;
                position: relative;
                left: 250px;
            }
            .box-2 {
                height: 400px;
                width: 400px;
                border: 3px solid #00d5ff;
                border-radius: 20px;
                background: transparent;
                position: relative;
                left: 300px;
            }
            .box-1 form {
                display: flex;
                color: white;
                background: transparent;
                padding: 10px;
                font-size: 15px;
                position: relative;
                top: 15px;
            }
            .box-1 form input {
                background: transparent;
                display: flex;
                border: 1px solid white;
                border-radius: 10px;
                padding: 15px 30px;
                font-size: 15px;
                color: white;
                position: relative;
                top: 30px;
            }
            .box-1 form textarea {
                background: transparent;
                color: white;
                padding: 15px 10px;
                position: relative;
                top: 30px;
                left: 30px;
                border: 1px solid white;
                border-radius: 10px;
            }
            .box-1 form button {
                border: 0;
                outline: none;
                padding: 10px 20px;
                color: white;
                border-radius: 30px;
                background: #00d5ff;
                cursor: pointer;
                position: relative;
                top: 50px;
            }
            .box-2 h2 {
                color: white;
                position: relative;
                top: 25px;
                left: 50px;
                font-size: 30px;
            }
            .box-2 p {
                color: white;
                position: relative;
                top: 50px;
                padding: 10px 80px;
            }
            .box-2 span {
                color: #00d5ff;
                font-size: 20px;
            }
        </style>
    </head>
    <body style="background-color: #6eded5;">
    <div class="banner">
        <br>
        <div class="navbar">
            <h1 style="color: white;">SAN PRODUCTS</h1>
            <ul>
                <li><a href="home.html"> Home </a></li>
                <li><a href="product.html"> Products </a></li>
                <li><a href="people.html"> People </a></li>
                <li><a href="contact.html"> Contact </a></li>
            </ul>
        </div>
        <div class="box">
            <div class="box-1">
                <form>
                    <center>
                        <h1> Contact Us </h1>
                        <input type="text" placeholder="Your Name">
                        <br>
                        <input type="email" placeholder="Your Email">
                        <br>
                        <button type="submit" > Submit </button>
                    </center>
                </form>
            </div>
            <div class="box-2"> 
                <h2> Contact Information </h2>
                <p> <span>Address</span> : 23/23 SEC, Thandlam, Chennai  </p>
                <p> <span>Email</span> : abc@gmail.com </p>
                <p> <span>Phone</span> : 938222*%*! </p>
            </div>
        </div>
    </div>
    <footer>
        <center>Developed by SANJAY S (212221243002) </center>
    </footer>
</body>
</html>
```

### CSS
```CSS
* {
    margin: 0;
    padding: 0;
    font-family: Arial, Helvetica, sans-serif;
}
.banner {
    width: 100%;
    height: 100vh;
    background-image: linear-gradient(rgba(173, 236, 181, 0.675),rgba(0,0,0,0.75)),url(background.jpg);
    background-size: cover;
    background-position: center;
}
.navbar {
    width: 85%;
    margin: auto;
    padding: 35px 0;
    display: flex;
    align-items: center;
    justify-content: space-between;
}
::placeholder {
    color: white;
}
footer {
    background-color: #ffffff;
    margin-top: auto;
    font-size: 20px;
}
```

## OUTPUT:
### HOME
![alt text](<Screenshot (80).png>)

### PRODUCT
![alt text](<Screenshot (81).png>)

### PEOPLE
![alt text](<Screenshot (82).png>)

### CONTACT
![alt text](<Screenshot (83).png>)

## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
