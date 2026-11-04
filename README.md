# Ex02 Commercial Website
## Date:04-11-2026

## AIM
To create a commercial website using CSS Flexbox.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for Homepage, Products / Services, About Us, Contact Details and User Account.

### STEP 5
Include social media links at the footer with copyright information.

### STEP 6
Define global styles for fonts, colors, and layout.

### STEP 7
Style the header, navigation bar, and sections.

### STEP 8
Use Flexbox for layout design.

### STEP 9
Add hover effects and transitions for interactivity.

### STEP 10
Add Images and Media.

### STEP 11
Use optimized images for a professional look.

### STEP 12
Open the HTML file in a browser to check layout and functionality.

### STEP 13
Fix styling issues and refine content placement.

### STEP 14
Deploy the website.

### STEP 15
Upload to GitHub Pages for free hosting.

## PROGRAM
index.html:
```c

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ShopEase - Online Shopping</title>
    <link rel="stylesheet" href="style.css">
</head>

<body>

    <!-- Header -->
    <header>
        <h1>ShopEase</h1>

        <nav>
            <a href="#home">Home</a>
            <a href="#products">Products</a>
            <a href="#about">About Us</a>
            <a href="#contact">Contact</a>
            <a href="#account">My Account</a>
        </nav>
    </header>

    <!-- Home -->
    <section id="home" class="home">
        <div class="home-content">
            <h2>Welcome to ShopEase</h2>
            <h3>Discover Amazing Products</h3>
            <p>Find the best products at affordable prices.
               Shop your favourite items today!</p>
            <a href="#products" class="btn">Shop Now</a>
        </div>
    </section>

    <!-- Products -->
    <section id="products">
        <h2>Our Products</h2>

        <div class="product-container">

            <div class="product">
                <img src="https://images.unsplash.com/photo-1598033129183-c4f50c736f10?w=500" alt="Men's Shirt">
                <h3>Men's Shirt</h3>
                <p>Price: ₹599</p>
                <button>Buy Now</button>
            </div>

            <div class="product">
                <img src="https://images.unsplash.com/photo-1542291026-7eec264c27ff?w=500" alt="Sports Shoes">
                <h3>Sports Shoes</h3>
                <p>Price: ₹999</p>
                <button>Buy Now</button>
            </div>

            <div class="product">
                <img src="https://images.unsplash.com/photo-1523275335684-37898b6baf30?w=500" alt="Watch">
                <h3>Smart Watch</h3>
                <p>Price: ₹1499</p>
                <button>Buy Now</button>
            </div>

            <div class="product">
                <img src="https://images.unsplash.com/photo-1548036328-c9fa89d128fa?w=500" alt="Hand Bag">
                <h3>Hand Bag</h3>
                <p>Price: ₹799</p>
                <button>Buy Now</button>
            </div>

        </div>
    </section>

    <!-- About -->
    <section id="about" class="about">
        <h2>About Us</h2>
        <p>
            ShopEase is an online shopping website that provides
            high-quality products at affordable prices.
            Our mission is to make online shopping easy,
            comfortable and convenient for everyone.
        </p>
    </section>

    <!-- Contact -->
    <section id="contact" class="contact">
        <h2>Contact Us</h2>
        <p>Email: support@shopease.com</p>
        <p>Phone: 9876543210</p>
        <p>Location: Chennai, Tamil Nadu</p>
    </section>

    <!-- User Account -->
    <section id="account" class="account">
        <h2>User Account</h2>

        <form>
            <label>Username:</label>
            <input type="text" placeholder="Enter username" required>

            <label>Password:</label>
            <input type="password" placeholder="Enter password" required>

            <button type="submit">Login</button>
        </form>
    </section>

    <!-- Footer -->
    <footer>
        <h3>ShopEase</h3>
        <p>Follow us on social media</p>

        <div class="social">
            <a href="https://www.instagram.com/">Instagram</a>
            <a href="https://www.facebook.com/">Facebook</a>
            <a href="https://www.youtube.com/">YouTube</a>
        </div>

        <p>© 2026 ShopEase. All Rights Reserved.</p>
    </footer>

</body>
</html>
```
style.css:
```c

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: Arial, sans-serif;
}

html {
    scroll-behavior: smooth;
}

body {
    background-color: #f5f5f5;
    color: #333;
}

/* Header */
header {
    background-color: #172554;
    color: white;
    padding: 20px 40px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
}

header h1 {
    font-size: 30px;
}

/* Navigation */
nav {
    display: flex;
    gap: 25px;
}

nav a {
    color: white;
    text-decoration: none;
    transition: 0.3s;
}

nav a:hover {
    color: #facc15;
}

/* Home */
.home {
    height: 400px;
    background: linear-gradient(120deg, #dbeafe, #bfdbfe);
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    padding: 30px;
}

.home-content h2 {
    font-size: 40px;
    color: #172554;
    margin-bottom: 15px;
}

.home-content h3 {
    font-size: 25px;
    margin-bottom: 15px;
}

.home-content p {
    margin-bottom: 25px;
    line-height: 1.6;
}

/* Button */
.btn {
    background-color: #172554;
    color: white;
    padding: 12px 25px;
    text-decoration: none;
    border-radius: 5px;
}

.btn:hover {
    background-color: #2563eb;
}

/* Sections */
section {
    padding: 50px 8%;
    text-align: center;
}

section h2 {
    color: #172554;
    font-size: 30px;
    margin-bottom: 30px;
}

/* Product Flexbox */
.product-container {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 25px;
}

/* Product Cards */
.product {
    background-color: white;
    width: 220px;
    padding: 15px;
    border-radius: 10px;
    box-shadow: 0 3px 10px #ccc;
    transition: 0.3s;
}

.product img {
    width: 100%;
    height: 180px;
    object-fit: cover;
    border-radius: 8px;
}

.product h3 {
    margin: 15px 0;
    color: #172554;
}

.product p {
    margin-bottom: 15px;
    font-weight: bold;
}

.product:hover {
    transform: translateY(-10px);
    box-shadow: 0 5px 15px #999;
}

/* Product Button */
.product button {
    background-color: #172554;
    color: white;
    padding: 10px 20px;
    border: none;
    border-radius: 5px;
    cursor: pointer;
}

.product button:hover {
    background-color: #2563eb;
}

/* About */
.about {
    background-color: #dbeafe;
}

.about p {
    line-height: 1.8;
}

/* Contact */
.contact {
    background-color: white;
    line-height: 2;
}

/* Account */
.account {
    background-color: #dbeafe;
}

.account form {
    max-width: 350px;
    margin: auto;
    display: flex;
    flex-direction: column;
    gap: 12px;
    text-align: left;
}

.account input {
    padding: 12px;
    border: 1px solid #aaa;
    border-radius: 5px;
}

.account button {
    padding: 12px;
    background-color: #172554;
    color: white;
    border: none;
    cursor: pointer;
}

/* Footer */
footer {
    background-color: #172554;
    color: white;
    text-align: center;
    padding: 25px;
    line-height: 2;
}

.social {
    display: flex;
    justify-content: center;
    gap: 25px;
}

.social a {
    color: #facc15;
    text-decoration: none;
}

.social a:hover {
    color: white;
}

/* Responsive Design */
@media (max-width: 600px) {
    header {
        flex-direction: column;
        gap: 20px;
    }

    nav {
        flex-wrap: wrap;
        justify-content: center;
    }

    .home-content h2 {
        font-size: 28px;
    }

    .product-container {
        flex-direction: column;
        align-items: center;
    }
}
```

## OUTPUT
![alt text](<Screenshot 2026-11-04 101621.png>)
![alt text](<Screenshot 2026-11-04 101707.png>)
![alt text](<Screenshot 2026-11-04 101729.png>)

## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
