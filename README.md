# Ex.07 Restaurant Website
## Date: 13/12/24

## AIM:
To develop a static Restaurant website to display the food items and services provided by them.

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
```
home.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Taste of Italy</title>
    <link rel="stylesheet" href="styles.css">
    <link rel="icon" href="favicon.ico" type="image/x-icon">
    <style>
        body {
            font-family: 'Roboto', sans-serif;
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            background-color: #f4f4f4;
            color: #333;
        }
        header {
            background: linear-gradient(135deg, #243b55, #141e30);
            color: white;
            text-align: center;
            padding: 60px 20px;
        }
        header h1 {
            font-size: 3em;
            margin-bottom: 10px;
        }
        nav ul {
            list-style: none;
            display: flex;
            justify-content: center;
            background: #243b55;
            margin: 0;
            padding: 10px;
        }
        nav ul li {
            margin: 0 20px;
        }
        nav ul li a {
            text-decoration: none;
            color: white;
            font-weight: bold;
            transition: color 0.3s;
        }
        nav ul li a:hover {
            color: #00a8cc;
        }
        main {
            padding: 20px;
            text-align: center;
        }
        #home {
            background: url('back.jpg') no-repeat center center/cover;
            color: white;
            padding: 60px 20px;
            border-radius: 8px;
            margin-bottom: 40px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            position: relative;
        }
        #home::after {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: rgba(0, 0, 0, 0.5);
            border-radius: 8px;
            z-index: 0;
        }
        #home h2, #home p, #home .cta-buttons {
            position: relative;
            z-index: 1;
        }
        #home h2 {
            font-size: 2.5em;
            margin-bottom: 20px;
        }
        #home p {
            font-size: 1.2em;
            margin-bottom: 30px;
        }
        .cta-buttons {
            display: flex;
            justify-content: center;
            gap: 20px;
        }
        .cta-buttons a {
            display: inline-block;
            padding: 10px 20px;
            color: white;
            background-color: #00a8cc;
            border-radius: 4px;
            text-decoration: none;
            font-weight: bold;
            transition: background 0.3s;
        }
        .cta-buttons a:hover {
            background-color: #005f73;
        }
        
        .featured-dishes {
            margin: 40px auto;
            display: flex;
            justify-content: space-between;
            gap: 20px;
            max-width: 1200px;
        }
        .dish, .opening-hours {
            flex: 1;
            background-color: #ffffff;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            text-align: center;
            transition: transform 0.3s;
        }
        .dish:hover, .opening-hours:hover {
            transform: translateY(-5px);
        }
        .dish {
            background-color: #005f73; 
        }
        .opening-hours {
            background-color: #ffe0b2;
        }
        .dish img {
            width: 100%;
            aspect-ratio: 3 / 4;
            object-fit: cover;
            border-radius: 8px;
        }
        .dish h4, .opening-hours h4 {
            margin-top: 10px;
            font-size: 1.5em;
            color: #243b55;
        }
        .opening-hours h3 {
            font-size: 1.8em;
            margin-bottom: 15px;
            color: #141e30;
        }
        .opening-hours p {
            font-size: 1.2em;
            margin: 5px 0;
        }
    </style>
</head>
<body>
    <header>
        <h1>Welcome to Taste of Italy</h1>
        <p>Your Culinary Journey Starts Here</p>
    </header>
    <nav>
        <ul>
            <li><a href="home.html">Home</a></li>
            <li><a href="menu.html">Menu</a></li>
            <li><a href="administration.html">Administration</a></li>
            <li><a href="contact.html">Contact Us</a></li>
        </ul>
    </nav>

    <main>
        <section id="home">
            <h2>Welcome to Our Website</h2>
            <p>Experience the best food and exceptional service in a cozy and inviting atmosphere. Explore our menu and discover your next favorite dish!</p>
            <div class="cta-buttons">
                <a href="menu.html">Explore Menu</a>
                <a href="contact.html">Reserve a Table</a>
            </div>
        </section>

        <h2>Today's Special</h2>

        <section class="featured-dishes">
            <div class="dish">
                <img src="dish1.jpg" alt="Dish 1">
                <h4 style="color: #f4f4f4;">Spaghetti Carbonara</h4>
                <p style="color: #f4f4f4;">A classic Italian pasta dish with creamy egg sauce, pancetta, and Parmesan cheese. Perfect for a cozy dinner!</p>
            </div>
            <div class="dish">
                <img src="dish2.jpg" alt="Dish 2">
                <h4 style="color: #f4f4f4;">Grilled Salmon</h4>
                <p style="color: #f4f4f4;">Succulent grilled salmon served with a fresh lemon herb butter sauce. A healthy and delicious choice!</p>
            </div>
            <div class="opening-hours">
                <h3>Opening Hours</h3>
                <p>Monday - Friday: 9:00 AM - 10:00 PM</p>
                <p>Saturday - Sunday: 10:00 AM - 11:00 PM</p>
            </div>
        </section>
    </main>

    <footer>
        <p>© 2024 Food Delight. All Rights Reserved.</p>
        <p>Website created by Harshul SL</p>
    </footer>
</body>
</html>

menu.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Menu</title>
    <link rel="stylesheet" href="styles.css">
    <link rel="icon" href="favicon.ico" type="image/x-icon">
    <style>
        body {
            font-family: 'Roboto', sans-serif;
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            background-color: #f4f4f4;
            color: #333;
        }
        header {
            background: linear-gradient(135deg, #243b55, #141e30);
            color: white;
            text-align: center;
            padding: 60px 20px;
        }
        header h1 {
            font-size: 3em;
            margin-bottom: 10px;
        }
        nav ul {
            list-style: none;
            display: flex;
            justify-content: center;
            background: #243b55;
            margin: 0;
            padding: 30px;
        }
        nav ul li {
            margin: 0 20px;
        }
        nav ul li a {
            text-decoration: none;
            color: white;
            font-weight: bold;
            transition: color 0.3s;
        }
        nav ul li a:hover {
            color: #00a8cc;
        }
        main {
            padding: 20px;
            text-align: center;
        }
        #menu {
            padding: 60px 20px;
            text-align: center;
        }
        #menu h2 {
            font-size: 2.5em;
            margin-bottom: 20px;
            color: #243b55;
        }
        .menu-row {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            margin-bottom: 20px;
        }
        .menu-item {
            background-color: #e0f7fa; /* Light teal background for menu items */
            padding: 10px;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            margin: 5px;
            transition: transform 0.3s;
            flex: 1 1 calc(25% - 20px); /* 4 items in a row with 20px gap */
            max-width: 300px; /* Limit the width */
        }
        .menu-item:hover {
            transform: translateY(-5px);
        }
        .menu-item img {
            width: 100%;
            aspect-ratio: 3 / 4; /* Maintain 3:4 ratio */
            object-fit: cover;
            border-radius: 8px;
        }
        .menu-item h3 {
            margin-top: 5px;
            font-size: 1.2em;
            color: #243b55;
        }
        .menu-item p {
            font-size: 1em;
            margin: 5px 0;
        }
        .menu-row {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            margin-bottom: 20px;
        }
        .menu-row > div {
            flex: 1 1 calc(33.333% - 20px);
            box-sizing: border-box;
        }
        footer {
            background: #141e30;
            color: white;
            text-align: center;
            padding: 20px;
        }
    </style>
</head>
<body>
   
    <nav>
        <ul>
            <li><a href="home.html">Home</a></li>
            <li><a href="menu.html">Menu</a></li>
            <li><a href="administration.html">Administration</a></li>
            <li><a href="contact.html">Contact Us</a></li>
        </ul>
    </nav>

    <main>
        <section id="menu">
            <h2>Our Menu</h2>

            <div class="menu-row">
                <div class="menu-item">
                    <img src="dish5.jpg" alt="Dish 5">
                    <h3>Chicken Alfredo</h3>
                    <p>Creamy Alfredo sauce with grilled chicken on fettuccine pasta.</p>
                    <p>Price: ₹1,700</p>
                </div>
                <div class="menu-item">
                    <img src="dish6.jpg" alt="Dish 6">
                    <h3>Veggie Stir-fry</h3>
                    <p>Stir-fried seasonal vegetables with soy sauce and a hint of garlic.</p>
                    <p>Price: ₹1,300</p>
                </div>
                <div class="menu-item">
                    <img src="dish7.jpg" alt="Dish 7">
                    <h3>Beef Burger</h3>
                    <p>Juicy beef patty with lettuce, tomato, and cheese in a toasted bun.</p>
                    <p>Price: ₹1,600</p>
                </div>
                <div class="menu-item">
                    <img src="dish8.jpg" alt="Dish 8">
                    <h3>Thai Green Curry</h3>
                    <p>Traditional Thai green curry with chicken, vegetables, and coconut milk.</p>
                    <p>Price: ₹1,900</p>
                </div>
                <div class="menu-item">
                    <img src="dish9.jpg" alt="Dish 9">
                    <h3>Beef Tacos</h3>
                    <p>Soft tortillas filled with seasoned beef, salsa, and cheese.</p>
                    <p>Price: ₹1,500</p>
                </div>
                <div class="menu-item">
                    <img src="dish10.jpg" alt="Dish 10">
                    <h3>Grilled Vegetables</h3>
                    <p>Freshly grilled vegetables served with a balsamic reduction.</p>
                    <p>Price: ₹1,400</p>
                </div>
                <div class="menu-item">
                    <img src="dish11.jpg" alt="Dish 11">
                    <h3>Classic Tiramisu</h3>
                    <p>Layered Italian dessert with mascarpone, coffee, and cocoa.</p>
                    <p>Price: ₹800</p>
                </div>
                <div class="menu-item">
                    <img src="dish12.jpg" alt="Dish 12">
                    <h3>Chocolate Lava Cake</h3>
                    <p>Rich chocolate cake with a gooey center, served with vanilla ice cream.</p>
                    <p>Price: ₹900</p>
                </div>
                <div class="menu-item">
                    <img src="dish13.jpg" alt="Dish 13">
                    <h3>Vegetarian Quesadilla</h3>
                    <p>Cheese and vegetable-filled quesadilla served with guacamole and sour cream.</p>
                    <p>Price: ₹1,400</p>
                </div>
                <div class="menu-item">
                    <img src="dish14.jpg" alt="Dish 14">
                    <h3>Beef Empanadas</h3>
                    <p>Flaky pastry filled with spiced beef, served with a tangy dipping sauce.</p>
                    <p>Price: ₹1,200</p>
                </div>
                <div class="menu-item">
                    <img src="dish15.jpg" alt="Dish 15">
                    <h3>Seafood Paella</h3>
                    <p>Spanish rice dish with shrimp, mussels, and clams, infused with saffron.</p>
                    <p>Price: ₹2,200</p>
                </div>
                <div class="menu-item">
                    <img src="dish16.jpg" alt="Dish 16">
                    <h3>Mango Sticky Rice</h3>
                    <p>Sweet and creamy dessert with fresh mango, sticky rice, and coconut milk.</p>
                    <p>Price: ₹700</p>
                </div>
            </div>
        </section>
    </main>

    <footer>
        <p>© 2024 Food Delight. All Rights Reserved.</p>
        <p>Website created by Harshul SL</p>
    </footer>
</body>
</html>

adminstration.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Administration - Food Delight</title>
    <link rel="stylesheet" href="styles.css">
    <link rel="icon" href="favicon.ico" type="image/x-icon">
    <style>
        body {
            font-family: 'Roboto', sans-serif;
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            background-color: #f4f4f4;
            color: #333;
        }
        header {
            background: linear-gradient(135deg, #243b55, #141e30);
            color: white;
            text-align: center;
            padding: 60px 20px;
        }
        header h1 {
            font-size: 3em;
            margin-bottom: 10px;
        }
        nav ul {
            list-style: none;
            display: flex;
            justify-content: center;
            background: #243b55;
            margin: 0;
            padding: 10px;
        }
        nav ul li {
            margin: 0 20px;
        }
        nav ul li a {
            text-decoration: none;
            color: white;
            font-weight: bold;
            transition: color 0.3s;
        }
        nav ul li a:hover {
            color: #00a8cc;
        }
        main {
            padding: 20px;
            text-align: center;
        }
        #administration {
            padding: 60px 20px;
            text-align: center;
        }
        #administration h2 {
            font-size: 2.5em;
            margin-bottom: 20px;
            color: #243b55;
        }
        .members {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
        }
        .member {
            background-color: #e0f7fa; /* Light teal background for member cards */
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            margin: 20px;
            text-align: center;
            transition: transform 0.3s;
            flex: 1 1 calc(25% - 40px); /* 4 items per row, with 20px gap */
            max-width: 250px; /* Limit the width */
        }
        .member:hover {
            transform: translateY(-5px);
        }
        .member img {
            width: 100px;
            height: 100px;
            border-radius: 50%;
            margin-bottom: 10px;
        }
        .member h3 {
            font-size: 1.5em;
            color: #243b55;
        }
        .member p {
            font-size: 1.2em;
            color: #333;
        }
        footer {
            background: #141e30;
            color: white;
            text-align: center;
            padding: 20px;
        }
    </style>
</head>
<body>
    <header>
        <h1>Administration - Taste Of Italy</h1>
        <p>Meet our dedicated team members!</p>
    </header>
    <nav>
        <ul>
            <li><a href="home.html">Home</a></li>
            <li><a href="menu.html">Menu</a></li>
            <li><a href="administration.html">Administration</a></li>
            <li><a href="contact.html">Contact Us</a></li>
        </ul>
    </nav>

    <main>
        <section id="administration">
            <h2>Meet Our Team</h2>

            <div class="members">
                <div class="member">
                    <img src="mem1.jpg" alt="Celebrity 1">
                    <h3>Chris Hemsworth</h3>
                    <p>CEO & Founder</p>
                </div>
                <div class="member">
                    <img src="mem2.jpg" alt="Celebrity 2">
                    <h3>Ryan Reynolds</h3>
                    <p>Marketing Director</p>
                </div>
                <div class="member">
                    <img src="mem3.jpg" alt="Celebrity 3">
                    <h3>Robert Downey Jr.</h3>
                    <p>Operations Manager</p>
                </div>
                <div class="member">
                    <img src="mem4.jpg" alt="Celebrity 4">
                    <h3>Tom Hiddleston</h3>
                    <p>Chef & Head Cook</p>
                </div>
                <div class="member">
                    <img src="mem5.jpg" alt="Celebrity 5">
                    <h3>Tom Cruise</h3>
                    <p>Customer Relations</p>
                </div>
                <div class="member">
                    <img src="mem6.jpg" alt="Celebrity 6">
                    <h3>Brad Pitt</h3>
                    <p>Executive Chef</p>
                </div>
            </div>
        </section>
    </main>

    <footer>
        <p>© 2024 Food Delight. All Rights Reserved.</p>
        <p>Website created by Harshul SL</p>
    </footer>
</body>
</html>

contact.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contact Us</title>
    <link rel="stylesheet" href="styles.css">
    <link rel="icon" href="favicon.ico" type="image/x-icon">
    <style>
        body {
            font-family: 'Roboto', sans-serif;
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            background-color: #f4f4f4;
            color: #333;
        }
        header {
            background: linear-gradient(135deg, #243b55, #141e30);
            color: white;
            text-align: center;
            padding: 60px 20px;
        }
        header h1 {
            font-size: 3em;
            margin-bottom: 10px;
        }
        nav ul {
            list-style: none;
            display: flex;
            justify-content: center;
            background: #243b55;
            margin: 0;
            padding: 10px;
        }
        nav ul li {
            margin: 0 20px;
        }
        nav ul li a {
            text-decoration: none;
            color: white;
            font-weight: bold;
            transition: color 0.3s;
        }
        nav ul li a:hover {
            color: #00a8cc;
        }
        main {
            padding: 20px;
            text-align: center;
        }
        #contact {
            padding: 60px 20px;
            text-align: center;
        }
        #contact h2 {
            font-size: 2.5em;
            margin-bottom: 20px;
            color: #243b55;
        }
        .contact-info {
            display: flex;
            justify-content: space-around;
            flex-wrap: wrap;
            margin-bottom: 30px;
        }
        .contact-info div {
            flex: 1 1 calc(33.333% - 40px);
            max-width: 300px;
            margin: 10px;
        }
        .contact-info div i {
            font-size: 2em;
            margin-bottom: 10px;
            color: #243b55;
        }
        .contact-info div h3 {
            font-size: 1.5em;
            margin-bottom: 5px;
        }
        .contact-info div p {
            font-size: 1em;
            color: #666;
        }
        .contact-form {
            max-width: 600px;
            margin: 0 auto;
            background-color: #e0f7fa; /* Light teal background */
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }
        .contact-form input,
        .contact-form textarea {
            width: calc(100% - 20px);
            padding: 10px;
            margin: 5px 0 15px 0;
            border: 1px solid #ddd;
            border-radius: 4px;
            box-sizing: border-box;
        }
        .contact-form button {
            width: 100%;
            padding: 10px;
            background-color: #243b55;
            color: white;
            border: none;
            border-radius: 4px;
            font-size: 1.2em;
            cursor: pointer;
            transition: background-color 0.3s;
        }
        .contact-form button:hover {
            background-color: #141e30;
        }
        footer {
            background: #141e30;
            color: white;
            text-align: center;
            padding: 20px;
        }
    </style>
</head>
<body>
    <header>
        <h1>Contact Us - Taste Of Italy</h1>
        <p>We'd love to hear from you! Reach out to us using the form below.</p>
    </header>
    <nav>
        <ul>
            <li><a href="home.html">Home</a></li>
            <li><a href="menu.html">Menu</a></li>
            <li><a href="administration.html">Administration</a></li>
            <li><a href="contact.html">Contact Us</a></li>
        </ul>
    </nav>

    <main>
        <section id="contact">
            <h2>Contact Information</h2>
            <div class="contact-info">
                <div>
                    <i class="fas fa-map-marker-alt"></i>
                    <h3>Address</h3>
                    <p>123 Food Street, Thirumullaivoyal, Ch 600062</p>
                </div>
                <div>
                    <i class="fas fa-phone-alt"></i>
                    <h3>Phone</h3>
                    <p>+1 (123) 456-7890</p>
                </div>
                <div>
                    <i class="fas fa-envelope"></i>
                    <h3>Email</h3>
                    <p>info@fooddelight.com</p>
                </div>
            </div>

            <h2>Send Us a Message</h2>
            <form class="contact-form">
                <input type="text" name="name" placeholder="Your Name" required>
                <input type="email" name="email" placeholder="Your Email" required>
                <textarea name="message" rows="5" placeholder="Your Message" required></textarea>
                <button type="submit">Send Message</button>
            </form>
        </section>
    </main>

    <footer>
        <p>© 2024 Food Delight. All Rights Reserved.</p>
        <p>Website created by HARSHUL SL</p>
    </footer>

    
</body>
</html>

```

## OUTPUT:

![alt text](<Screenshot (21).png>)
![alt text](<Screenshot (22).png>)
![alt text](<Screenshot (23).png>)
![alt text](<Screenshot (24).png>)
![alt text](<Screenshot (25).png>)
![alt text](<Screenshot (26).png>)


## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
