# Ex02 Commercial Website

## Date:15/03/2025

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
#home.html
```
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <header>
      <nav>
        <ul class="navbar">
          <li><a href="home.html">Home</a></li>
          <li><a href="products.html">Products</a></li>
          <li><a href="about.html">About Us</a></li>
          <li><a href="contact.html">Contact</a></li>
          <li><a href="login.html">Login</a></li>
          <li><a href="sign.html">Sign Up</a></li>
        </ul>
      </nav>
    </header>

    <section id="home" class="section active">
      <h1>Welcome to Our Website!</h1>
      <p>
        Your one-stop shop for quality products, unbeatable prices, and
        outstanding service.
      </p>
      <button class="cta-button" onclick="showSection('products')">
        Shop Now
      </button>
    </section>
    <section id="contact" class="section">
      <h2>Contact Us</h2>
      <p>Email: support@yourcompany.com | Phone: +123-456-7890</p>
    </section>
    <footer>
      <div class="socials">
        <a href="https://facebook.com" target="_blank">Facebook</a>
        <a href="https://twitter.com" target="_blank">Twitter</a>
        <a href="https://instagram.com" target="_blank">Instagram</a>
      </div>
      <p>&copy; 2025 Your Company. All rights reserved.</p>
    </footer>
  </body>
</html>


```
product.html
```
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <header>
      <nav>
        <ul class="navbar">
          <li><a href="home.html">Home</a></li>
          <li><a href="products.html">Products</a></li>
          <li><a href="about.html">About Us</a></li>
          <li><a href="contact.html">Contact</a></li>
          <li><a href="login.html">Login</a></li>
          <li><a href="sign.html">Sign Up</a></li>
        </ul>
      </nav>
    </header>

    
      <h2>Our Products and Services</h2>
      <div class="product-grid">
        <div class="product-card">
          <img src="images.jpeg" alt="Product 1" />
          <h3>Product 1</h3>
          <p>High-quality item that meets your needs.</p>
        </div>
        <div class="product-card">
          <img
            src="pexels-nathalia-djaleska-2148956646-30358745.jpg"
            alt="Product 2"
          />
          <h3>Product 2</h3>
          <p>Top-rated service trusted by thousands.</p>
        </div>
      </div>
    </section>
    <section id="contact" class="section">
      <h2>Contact Us</h2>
      <p>Email: support@yourcompany.com | Phone: +123-456-7890</p>
    </section>
    <footer>
      <div class="socials">
        <a href="https://facebook.com" target="_blank">Facebook</a>
        <a href="https://twitter.com" target="_blank">Twitter</a>
        <a href="https://instagram.com" target="_blank">Instagram</a>
      </div>
      <p>&copy; 2025 Your Company. All rights reserved.</p>
    </footer>
  </body>
</html>

```
#about.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="style.css" />
</head>
<body>
    <header>
        <nav>
          <ul class="navbar">
            <li><a href="home.html">Home</a></li>
            <li><a href="products.html">Products</a></li>
            <li><a href="about.html">About Us</a></li>
            <li><a href="contact.html">Contact</a></li>
            <li><a href="login.html">Login</a></li>
            <li><a href="sign.html">Sign Up</a></li>
          </ul>
        </nav>
      </header>
      <h2>About Us</h2>
      <p>
        We are committed to delivering the best products with outstanding
        customer service.
      </p>
    </section>
   
    <section id="contact" class="section">
      <h2>Contact Us</h2>
      <p>Email: support@yourcompany.com | Phone: +123-456-7890</p>
    </section>
    
    <footer>
        <div class="socials">
          <a href="https://facebook.com" target="_blank">Facebook</a>
          <a href="https://twitter.com" target="_blank">Twitter</a>
          <a href="https://instagram.com" target="_blank">Instagram</a>
        </div>
        <p>&copy; 2025 Your Company. All rights reserved.</p>
      </footer>
    
    
      <section id="about" class="section">
        
</body>
</html>
```
#contact.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="style.css" />
</head>
<body>
    <header>
        <nav>
          <ul class="navbar">
            <li><a href="home.html">Home</a></li>
            <li><a href="products.html">Products</a></li>
            <li><a href="about.html">About Us</a></li>
            <li><a href="contact.html">Contact</a></li>
            <li><a href="login.html">Login</a></li>
            <li><a href="sign.html">Sign Up</a></li>
          </ul>
        </nav>
      </header>
      
        <h2>Contact Us</h2>
        <p>Email: support@yourcompany.com | Phone: +123-456-7890</p>
        <footer>
            <div class="socials">
              <a href="https://facebook.com" target="_blank">Facebook</a>
              <a href="https://twitter.com" target="_blank">Twitter</a>
              <a href="https://instagram.com" target="_blank">Instagram</a>
            </div>
            <p>&copy; 2025 Your Company. All rights reserved.</p>
          </footer>
      
</body>
</html>
```
#css
```
html, body {
  height: 100%;
  margin: 0;
  display: flex;
  flex-direction: column;
}
.content {
  flex: 1;
}
body {
  font-family: Arial, sans-serif;
  background-color: #f5f5f5;
  color: #333;
  margin: 0;
  padding: 0;
  text-align: center;
}

/* Navigation Bar */
.navbar {
  display: flex;
  justify-content: center;
  background-color: #333;
  padding: 10px 0;
  list-style: none;
  margin: 0;
}

.navbar li {
  margin: 0 15px;
}

.navbar a {
  color: white;
  text-decoration: none;
  padding: 10px 20px;
  transition: background 0.3s ease;
  cursor: pointer;
}

.navbar a:hover {
  background: #555;
  border-radius: 5px;
}

/* Sections */
.section {
  display: none;
  padding: 20px;
}

.section.active {
  display: block;
}


.cta-button {
  padding: 12px 24px;
  background-color: #28a745;
  color: white;
  border: none;
  cursor: pointer;
  transition: background 0.3s ease;
}

.cta-button:hover {
  background-color: #218838;
}

/* Product Grid */
.product-grid {
  display: flex;
  justify-content: center;
  gap: 20px;
  flex-wrap: wrap;
}

.product-card {
  background: white;
  border-radius: 10px;
  padding: 15px;
  text-align: center;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  transition: transform 0.3s;
}

.product-card:hover {
  transform: scale(1.05);
}

.product-card img {
  width: 100px;
  height: auto;
}


footer {

  text-align: center;
  padding: 15px;
  background-color: #333;
  color: white;
  
}
footer {
  text-align: center;
  padding: 15px;
  background-color: #333;
  color: white;
  margin-top: auto; 
}

.socials a {
  color: white;
  margin: 0 10px;
  text-decoration: none;
  transition: color 0.3s;
}

.socials a:hover {
  color: #ddd;
}

}

```
## OUTPUT
## HOME
![image](https://github.com/user-attachments/assets/7ad2648a-a30d-471a-860b-182fe935c6df)

## PROUDUCTS
![image](https://github.com/user-attachments/assets/6fc9b466-f2f2-41fc-81c5-593c97de04e2)

## ABOUT US
![image](https://github.com/user-attachments/assets/06fe03e7-dda0-4027-9e5e-5c92961bd61a)

## CONTACT US
![image](https://github.com/user-attachments/assets/703c5d15-07b8-4ac9-89fe-7dfa5d06d4fc)






## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
