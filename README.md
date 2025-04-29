# Ex.07 Restaurant Website
## Date: 29/04/2025
## Name: Saravana Kuamr S
## Reg no: 212224220090

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
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>NK Restaurant</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f8f5f1;
            animation: backgroundAnimation 10s infinite alternate;
        }

        @keyframes backgroundAnimation {
            0% { background-color: #f8f5f1; }
            50% { background-color: #ffe4e1; }
            100% { background-color: #ffeadb; }
        }

        header {
            background-color: #ff6f61;
            color: white;
            text-align: center;
            padding: 20px;
            animation: headerAnimation 5s infinite alternate;
        }

        @keyframes headerAnimation {
            0% { background-color: #ff6f61; }
            50% { background-color: #ff8a75; }
            100% { background-color: #ffaf94; }
        }

        nav {
            background-color: #4a4a4a;
            overflow: hidden;
        }

        nav a {
            float: left;
            display: block;
            color: white;
            text-align: center;
            padding: 14px 20px;
            text-decoration: none;
            transition: background-color 0.3s;
        }

        nav a:hover {
            background-color: #ff6f61;
            color: white;
        }

        .banner {
            background-image: url('banner.jpg');
            background-size: cover;
            height: 300px;
            display: flex;
            justify-content: center;
            align-items: center;
            color: rgb(10, 1, 1);
            font-size: 2.5em;
            animation: textPulse 5s infinite alternate;
        }

        @keyframes textPulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.1); }
            100% { transform: scale(1); }
        }

        .content {
            padding: 20px;
        }

        .menu-items, .admin-section {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
            gap: 20px;
            margin-top: 20px;
        }

        .menu-item, .admin {
            border: 1px solid #ddd;
            border-radius: 8px;
            overflow: hidden;
            text-align: center;
            background-color: #fff;
            animation: fadeIn 2s ease-in;
        }

        @keyframes fadeIn {
            0% { opacity: 0; }
            100% { opacity: 1; }
        }

        .menu-item img, .admin img {
            width: 100%;
            height: 150px;
            object-fit: cover;
        }

        footer {
            text-align: center;
            background-color: #4a4a4a;
            color: white;
            padding: 10px;
            margin-top: 20px;
        }

        .contact {
            text-align: center;
            margin-top: 20px;
            background-color: #ffeed8;
            padding: 20px;
            animation: backgroundAnimation 10s infinite alternate;
        }
    </style>
</head>
<body>
    <header>
        <h1>Welcome to NK Restaurant</h1>
    </header>
    <nav>
        <a href="#home">Home</a>
        <a href="#menu">Menu</a>
        <a href="#administration">Administration</a>
        <a href="#contact">Contact Us</a>
    </nav>

    <div id="home" class="banner">
        <p>Delicious Food, Delivered Fresh</p>
    </div>

    <div id="menu" class="content">
        <h2>Our Menu</h2>
        <div class="menu-items">
            <div class="menu-item">
                <img src="grilled-chicken-recipe-best-5-of-6.jpg" alt="Dish 1">
                <p>Grilled Chicken</p>
            </div>
            <div class="menu-item">
                <img src="vegetable salad.jpg" alt="Dish 2">
                <p>Vegetable Salad</p>
            </div>
            <div class="menu-item">
                <img src="Pasta Alfredo.jpg" alt="Dish 3">
                <p>Pasta Alfredo</p>
            </div>
            <div class="menu-item">
                <img src="Margherita Pizza.webp" alt="Dish 4">
                <p>Margherita Pizza</p>
            </div>
            <div class="menu-item">
                <img src="Cheeseburger.jpg" alt="Dish 5">
                <p>Cheeseburger</p>
            </div>
            <div class="menu-item">
                <img src="Chocolate Cake.jpg" alt="Dish 6">
                <p>Chocolate Cake</p>
            </div>
            <div class="menu-item">
                <img src="Sushi Rolls.jpg" alt="Dish 7">
                <p>Sushi Rolls</p>
            </div>
            <div class="menu-item">
                <img src="Ice Cream Sundae.jpg" alt="Dish 8">
                <p>Ice Cream Sundae</p>
            </div>
            <div class="menu-item">
                <img src="Fish Tacos.jpg" alt="Dish 9">
                <p>Fish Tacos</p>
            </div>
            <div class="menu-item">
                <img src="Fried Rice.jpg" alt="Dish 10">
                <p>Fried Rice</p>
            </div>
            <div class="menu-item">
                <img src="Paneer Butter Masala.jpg" alt="Dish 11">
                <p>Paneer Butter Masala</p>
            </div>
            <div class="menu-item">
                <img src="Caesar Salad.jpg" alt="Dish 12">
                <p>Caesar Salad</p>
            </div>
        </div>
    </div>

    <div id="administration" class="content">
        <h2>Our Administration</h2>
        <div class="admin-section">
            <div class="admin">
                <img src="John Doe.jpg" alt="Admin 1">
                <p>John Doe - Manager</p>
            </div>
            <div class="admin">
                <img src="Jane Smith.jpg" alt="Admin 2">
                <p>Jane Smith - Chef</p>
            </div>
            <div class="admin">
                <img src="Emily Brown.jpg" alt="Admin 3">
                <p>Emily Brown - Sous Chef</p>
            </div>
            <div class="admin">
                <img src="Michael Green.jpg" alt="Admin 4">
                <p>Michael Green - Accountant</p>
            </div>
            <div class="admin">
                <img src="Sarah Wilson.jpg" alt="Admin 5">
                <p>Sarah Wilson - HR</p>
            </div>
            <div class="admin">
                <img src="Chris Taylor.jpg" alt="Admin 6">
                <p>Chris Taylor - Delivery Head</p>
            </div>
        </div>
    </div>

    <div id="contact" class="contact">
        <h2>Contact Us</h2>
        <p>Address: 123 Food Street, Taste Town</p>
        <p>Phone: (123) 456-7890</p>
        <p>Email: contact@nkrestaurant.com</p>
    </div>

    <footer>
        <p>Created by Saravana Kumar S</p>
    </footer>
</body>
</html>


```

## OUTPUT:

Screenshot 2024-12-14 202039

Screenshot 2024-12-14 202053

## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
