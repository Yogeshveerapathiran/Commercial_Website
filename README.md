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
```index
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link rel="stylesheet" href="style.css" />
    <title>Commercial Website</title>
  </head>
  <body>
    <header>
      <nav>
        <ul class="navbar">
          <li><a onclick="showSection('home')">Home</a></li>
          <li><a onclick="showSection('products')">Products</a></li>
          <li><a onclick="showSection('about')">About Us</a></li>
          <li><a onclick="showSection('contact')">Contact</a></li>
          <li><a onclick="openModal('auth-modal')">Login / Sign Up</a></li>
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

    <section id="products" class="section">
      <h2>Our Products and Services</h2>
      <div class="product-grid">
        <div class="product-card">
          <img src="optimized-product1.jpg" alt="Product 1" />
          <h3>Product 1</h3>
          <p>High-quality item that meets your needs.</p>
        </div>
        <div class="product-card">
          <img src="optimized-product2.jpg" alt="Product 2" />
          <h3>Product 2</h3>
          <p>Top-rated service trusted by thousands.</p>
        </div>
      </div>
    </section>

    <section id="about" class="section">
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

    <div id="auth-modal" class="modal">
      <div class="modal-content">
        <span class="close" onclick="closeModal('auth-modal')">&times;</span>
        <h2>Login / Sign Up</h2>
        <form id="auth-form">
          <input type="text" id="username" placeholder="Username" required />
          <input type="email" id="email" placeholder="Email" required />
          <input
            type="password"
            id="password"
            placeholder="Password"
            required
          />
          <button type="submit">Submit</button>
        </form>
      </div>
    </div>

    <div class="user-icon" onclick="openProfile()">
      <img src="user-icon.png" alt="User Profile" />
    </div>

    <div id="user-profile" class="profile-modal">
      <div class="profile-content">
        <span class="close" onclick="closeProfile()">&times;</span>
        <h2>User Profile</h2>
        <p id="profile-username">Username: Guest</p>
        <p id="profile-email">Email: Not Logged In</p>
      </div>
    </div>

    <script>
      function showSection(sectionId) {
        document
          .querySelectorAll(".section")
          .forEach((section) => section.classList.remove("active"));
        document.getElementById(sectionId).classList.add("active");
      }

      function openModal(modalId) {
        document.getElementById(modalId).style.display = "block";
      }

      function closeModal(modalId) {
        document.getElementById(modalId).style.display = "none";
      }

      function openProfile() {
        document.getElementById("user-profile").style.display = "block";
      }

      function closeProfile() {
        document.getElementById("user-profile").style.display = "none";
      }

      document
        .getElementById("auth-form")
        .addEventListener("submit", function (event) {
          event.preventDefault();
          const username = document.getElementById("username").value;
          const email = document.getElementById("email").value;
          document.getElementById("profile-username").innerText =
            "Username: " + username;
          document.getElementById("profile-email").innerText =
            "Email: " + email;
          closeModal("auth-modal");
        });
    </script>
  </body>
</html>

```
```css
body {
  font-family: Arial, sans-serif;
  margin: 0;
  padding: 0;
  text-align: center;
}

header {
  background-color: #333;
  padding: 10px 0;
}

.navbar {
  list-style: none;
  padding: 0;
  display: flex;
  justify-content: center;
}

.navbar li {
  margin: 0 15px;
}

.navbar a {
  color: white;
  text-decoration: none;
  cursor: pointer;
}

.section {
  display: none;
  padding: 50px;
}

.section.active {
  display: block;
}

.cta-button {
  background-color: #008cba;
  color: white;
  padding: 10px 20px;
  border: none;
  cursor: pointer;
}

.product-grid {
  display: flex;
  justify-content: center;
  gap: 20px;
  padding: 20px;
}

.product-card {
  border: 1px solid #ddd;
  padding: 15px;
  width: 200px;
}

.product-card img {
  width: 100%;
}

footer {
  background-color: #333;
  color: white;
  padding: 10px;
  margin-top: 20px;
}

.socials a {
  color: white;
  margin: 0 10px;
  text-decoration: none;
}

.modal,
.profile-modal {
  display: none;
  position: fixed;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  background-color: white;
  padding: 20px;
  border: 1px solid #ddd;
}

.close {
  cursor: pointer;
  float: right;
}

.user-icon {
  position: fixed;
  bottom: 20px;
  right: 20px;
  cursor: pointer;
}

.user-icon img {
  width: 50px;
}

```
## OUTPUT
## HOME
![image](https://github.com/user-attachments/assets/607bc86e-63c3-4a2b-be17-9caff9f13957)
## PROUDUCTS
![image](https://github.com/user-attachments/assets/18858c75-e5cb-4bff-b2e7-c43b80e06d98)
## ABOUT US
![image](https://github.com/user-attachments/assets/2f85ea5a-2a55-4291-9da0-d1f5b9dad338)
## CONTACT US
![image](https://github.com/user-attachments/assets/88e70091-cbac-4ccc-91fc-bf37a86a991f)
## SOCIAL MEDIA
![image](https://github.com/user-attachments/assets/5853f829-f415-42e4-839e-621cae7fbdfd)
## LOGIN/SIGNUP
![image](https://github.com/user-attachments/assets/cec4da79-daa8-4d01-9fec-c80c576f1a6f)
## USER DETAILS
![image](https://github.com/user-attachments/assets/44ad262f-f907-4191-b9b3-d73ff1a3a6b8)





## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
