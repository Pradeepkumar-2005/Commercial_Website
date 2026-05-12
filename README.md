# Ex02 Commercial Website
## Name:Pradeep kumar R
## Reg no: 212223220077
## Date:12/05/2026

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
index.html
```
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>CycleZone</title>
    <link rel="stylesheet" href="style.css" />
</head>

<body>

    <header class="header">
        <div class="logo">CycleZone</div>
        <nav class="navbar">
            <a href="#">Home</a>
            <a href="#bikes">Cycles</a>
            <a href="#about">About</a>
            <a href="#contact">Contact</a>
        </nav>
    </header>

    <section class="hero">
        <div class="hero-text">
            <h1>Find Your Perfect Ride</h1>
            <p>Shop the latest mountain, road, and city bikes at the best prices.</p>
            <a href="#bikes" class="btn">Shop Now</a>
        </div>
    </section>

    <section class="products" id="bikes">
        <h2>Our Cycles</h2>
        <div class="product-container">
            <div class="card">
                <img src="https://picsum.photos/300/200?random=1" alt="Mountain Bike">
                <h3>Mountain Bike</h3>
                <p>Strong frame and wide tires for off-road riding.</p>
                <div class="specs">21-Speed | Aluminum Frame | 26" Wheels</div>
                <span>₹18,999</span>
                <button>Buy Now</button>
            </div>

            <div class="card">
                <img src="https://picsum.photos/300/200?random=2" alt="Road Bike">
                <h3>Road Bike</h3>
                <p>Lightweight design built for speed and smooth roads.</p>
                <div class="specs">16-Speed | Carbon Frame | 700c Wheels</div>
                <span>₹24,499</span>
                <button>Buy Now</button>
            </div>

            <div class="card">
                <img src="https://picsum.photos/300/200?random=3" alt="City Bike">
                <h3>City Bike</h3>
                <p>Comfortable and stylish for daily commuting.</p>
                <div class="specs">7-Speed | Steel Frame | 26" Wheels</div>
                <span>₹15,750</span>
                <button>Buy Now</button>
            </div>
        </div>
    </section>

    <section class="features">
        <h2>Why Choose CycleZone?</h2>
        <div class="features-container">
            <div class="feature-card">
                <div class="feature-icon">✓</div>
                <h3>Curated Selection</h3>
                <p>We keep our catalog tight so the experience stays focused and useful.</p>
            </div>
            <div class="feature-card">
                <div class="feature-icon">✓</div>
                <h3>Responsive Support</h3>
                <p>Support is available across common channels whenever you need help.</p>
            </div>
            <div class="feature-card">
                <div class="feature-icon">✓</div>
                <h3>Secure Checkout</h3>
                <p>Transactions are designed to feel straightforward and dependable.</p>
            </div>
        </div>
    </section>

    <section class="about" id="about">
        <h2>About Us</h2>
        <p>CycleZone offers quality bicycles for every rider, from beginners to professionals. We've been committed to providing the best cycling experience for over a decade.</p>
    </section>

    <section class="contact-section" id="contact">
        <div class="contact-wrapper">
            <div class="contact-details">
                <h2>Contact Details</h2>
                <h3>Reach us when you need assistance.</h3>
                <p><strong>Email:</strong> support@cyclezone.com</p>
                <p><strong>Phone:</strong> +91 98765 43210</p>
                <p><strong>Address:</strong> 24 Commerce Avenue, India(Tamil Nadu)</p>
            </div>
            <div class="user-account">
                <h2>User Account</h2>
                <h3>Track orders, manage saved items, and update details.</h3>
                <form class="account-form">
                    <div class="form-group">
                        <label>Email address</label>
                        <input type="email" placeholder="you@example.com">
                    </div>
                    <div class="form-group">
                        <label>Password</label>
                        <input type="password" placeholder="Enter your password">
                    </div>
                    <button type="submit" class="signin-btn">Sign In</button>
                </form>
            </div>
        </div>
    </section>

    <footer class="footer">
        <p>Facebook Instagram X</p>
        <p>&copy; 2026 CycleZone. All rights reserved.</p>
    </footer>

</body>
</html>
```
style.css
```
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: Arial, sans-serif;
}

body {
    background-color: #f4f4f4;
    color: #222;
    line-height: 1.6;
}

.header {
    background: #0f172a;
    color: white;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px 50px;
    flex-wrap: wrap;
}

.logo {
    font-size: 28px;
    font-weight: bold;
}

.navbar {
    display: flex;
    gap: 20px;
    flex-wrap: wrap;
}

.navbar a {
    color: white;
    text-decoration: none;
    font-size: 16px;
}

.hero {
    background: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)),
        url('https://picsum.photos/1200/500?random=4') no-repeat center center/cover;
    color: white;
    text-align: center;
    padding: 100px 20px;
}

.hero h1 {
    font-size: 48px;
    margin-bottom: 15px;
}

.hero p {
    font-size: 20px;
    margin-bottom: 20px;
}

.btn {
    display: inline-block;
    background: #22c55e;
    color: white;
    padding: 12px 24px;
    text-decoration: none;
    border-radius: 5px;
}

.products {
    padding: 50px 20px;
    text-align: center;
}

.products h2 {
    font-size: 32px;
    margin-bottom: 30px;
}

.product-container {
    display: flex;
    justify-content: center;
    gap: 25px;
    flex-wrap: wrap;
}

.card {
    background: white;
    width: 300px;
    border-radius: 10px;
    overflow: hidden;
    box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
    padding-bottom: 20px;
}

.card img {
    width: 100%;
    height: 200px;
    object-fit: cover;
}

.card h3 {
    margin: 15px 0 10px;
}

.card p {
    padding: 0 15px;
    font-size: 14px;
    color: #555;
}

.specs {
    padding: 10px 15px;
    font-size: 12px;
    color: #888;
    background: #f9f9f9;
}

.card span {
    display: block;
    margin: 15px 0;
    font-size: 20px;
    font-weight: bold;
    color: #16a34a;
}

.card button {
    background: #0f172a;
    color: white;
    border: none;
    padding: 10px 20px;
    cursor: pointer;
    border-radius: 5px;
}

.about {
    background: #e2e8f0;
    padding: 50px 20px;
    text-align: center;
}

.about h2 {
    margin-bottom: 15px;
    font-size: 30px;
}

.features {
    padding: 50px 20px;
    background: white;
    text-align: center;
}

.features h2 {
    font-size: 32px;
    margin-bottom: 40px;
}

.features-container {
    display: flex;
    justify-content: center;
    gap: 30px;
    flex-wrap: wrap;
    max-width: 1000px;
    margin: 0 auto;
}

.feature-card {
    background: white;
    padding: 30px;
    border-radius: 10px;
    width: 280px;
    box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
    border-top: 3px solid #22c55e;
}

.feature-icon {
    font-size: 32px;
    color: #22c55e;
    font-weight: bold;
    margin-bottom: 15px;
}

.feature-card h3 {
    margin-bottom: 10px;
    font-size: 18px;
    color: #0f172a;
}

.feature-card p {
    font-size: 14px;
    color: #666;
    line-height: 1.5;
}

.contact-section {
    padding: 50px 20px;
    background: #f4f4f4;
}

.contact-wrapper {
    display: flex;
    justify-content: center;
    gap: 40px;
    flex-wrap: wrap;
    max-width: 1000px;
    margin: 0 auto;
}

.contact-details, .user-account {
    background: white;
    padding: 30px;
    border-radius: 10px;
    width: 400px;
    box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
}

.contact-details h2, .user-account h2 {
    font-size: 22px;
    margin-bottom: 10px;
    color: #22c55e;
    text-transform: uppercase;
    font-size: 12px;
    font-weight: bold;
    letter-spacing: 1px;
}

.contact-details h3, .user-account h3 {
    font-size: 20px;
    margin-bottom: 20px;
    color: #0f172a;
    font-weight: bold;
}

.contact-details p {
    margin-bottom: 15px;
    font-size: 14px;
    color: #555;
    line-height: 1.8;
}

.account-form {
    display: flex;
    flex-direction: column;
    gap: 15px;
}

.form-group {
    display: flex;
    flex-direction: column;
}

.form-group label {
    margin-bottom: 8px;
    font-size: 14px;
    font-weight: bold;
    color: #0f172a;
}

.form-group input {
    padding: 10px;
    border: 1px solid #ddd;
    border-radius: 5px;
    font-size: 14px;
}

.signin-btn {
    background: #22c55e;
    color: white;
    border: none;
    padding: 12px;
    border-radius: 5px;
    font-weight: bold;
    cursor: pointer;
    font-size: 16px;
}

.signin-btn:hover {
    background: #16a34a;
}

.footer {
    background: #0f172a;
    color: white;
    text-align: center;
    padding: 20px;
}

@media (max-width: 768px) {
    .header {
        flex-direction: column;
        text-align: center;
        gap: 15px;
    }

    .navbar {
        justify-content: center;
    }

    .hero h1 {
        font-size: 32px;
    }

    .hero p {
        font-size: 18px;
    }

    .features-container {
        flex-direction: column;
        align-items: center;
    }

    .feature-card {
        width: 100%;
        max-width: 350px;
    }

    .contact-wrapper {
        flex-direction: column;
        align-items: center;
    }

    .contact-details, .user-account {
        width: 100%;
        max-width: 400px;
    }
}
```
## OUTPUT
<img width="1888" height="910" alt="Screenshot 2026-05-12 103605" src="https://github.com/user-attachments/assets/6cdcd818-83f9-4755-b9db-a49bf32258f9" />
<img width="1896" height="911" alt="Screenshot 2026-05-12 103620" src="https://github.com/user-attachments/assets/35bbff6e-c15a-4863-8d8c-db4428d3887c" />
<img width="1883" height="886" alt="Screenshot 2026-05-12 103637" src="https://github.com/user-attachments/assets/d0c33ee7-7228-4fb2-8086-41315bad238c" />
<img width="1889" height="902" alt="Screenshot 2026-05-12 103706" src="https://github.com/user-attachments/assets/78d8f5e4-9c13-47ad-8c03-8b5c37cea470" />


## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
