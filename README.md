# Midterm
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title> Mokojin Cafe </title>
    <link rel="stylesheet" href="style.css">
    <style>
        body {
            font-family: 'Courier New', monospace;
            margin: 0;
            padding: 0;
        }
        .header {
            background-color: #8B4513;
            padding: 20px 0;
            text-align: center;
        }
        .header img {
            width: 200px;
            height: auto;
        }
        .nav {
            text-align: center;
            background-color: #D2B48C;
            padding: 10px 0;
        }
        .nav a {
            margin: 0 15px;
            text-decoration: none;
            font-size: 18px;
            color: white;
            font-weight: bold;
            padding: 10px;
        }
        .nav a.active {
            background-color: white;
            color: black;
            border-radius: 5px;
        }
        .content {
            position: relative;
            text-align: center;
            color: white;
            height: 100vh;
            background-image: url('images/cofeeshop.jpg');
            background-size: cover;
            background-position: center;
            background-attachment: fixed;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            padding: 0 20px;
        }
        .content::before {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.5);
            z-index: 0;
        }
        .content h3 {
            position: relative;
            z-index: 2;
            font-size: 14px;
            font-weight: 400;
            letter-spacing: 2px;
            text-transform: uppercase;
        }
        .content h1 {
            position: relative;
            z-index: 2;
            font-size: 50px;
            font-weight: 700;
            margin: 10px 0;
        }
        .content p {
            position: relative;
            z-index: 2;
            font-size: 16px;
            font-weight: 300;
            max-width: 800px;
            text-align: center;
            line-height: 1.6;
        }
    </style>
    <script>
        document.addEventListener("DOMContentLoaded", function() {
            const currentLocation = window.location.href;
            const navLinks = document.querySelectorAll(".nav a");
            navLinks.forEach(link => {
                if (link.href === currentLocation) {
                    link.classList.add("active");
                }
            });
        });
    </script>
</head>
<body>
    <div class="header">
        <img src="images/webdev-removebg-preview.png" alt="Header Logo">
    </div>

    <div class="nav">
        <a href="home.html">HOME</a>
        <a href="viewmenu.html">VIEW MENU</a>
        <a href="aboutus.html">ABOUT US</a>
        <a href="contactus.html">CONTACT US</a> 
    </div>

    <div class="content"> 
        <h3>CHAMPIONING SPECIALTY COFFEE AND THE BEST BRUNCH IN ASIA SINCE 2018</h3>
        <h1>True to Great Coffee and Good People</h1>
        <p>Mokojin Cafe Coffee Shop are led by a team dedicated to championing their love for specialty coffee in an approachable and enjoyable way.</p>    
    </div>
</body>
</html>
