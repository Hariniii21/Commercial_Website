# Ex02 Commercial Website
## Date:11.05.26

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

## index.html

```
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Harini Store</title>
<link rel="stylesheet" href="style.css">
</head>

<body>

<!-- NAVBAR -->
<header class="navbar">
<h2>Harini Store</h2>

<nav>
<a href="#home">Home</a>
<a href="#products">Products</a>
<a href="#about">About</a>
<a href="#contact">Contact</a>
</nav>
</header>

<!-- HOME SECTION -->
<section id="home" class="home">

<div class="home-content">
<h1>Welcome to Harini Store</h1>

<p>
Harini Store is your trusted online shopping destination offering
modern gadgets, smart accessories, and premium electronics at affordable prices.
We focus on quality, innovation, and customer satisfaction.
</p>

<p>
Explore our latest collection of smart watches, smartphones,
wireless accessories, and digital devices designed to simplify your lifestyle.
</p>

<a href="#products" class="btn">Shop Now</a>

</div>

</section>

<!-- PRODUCTS -->
<section id="products">

<h2 class="section-title">Our Products</h2>

<div class="products">

<div class="product-card">
<img src="https://images.unsplash.com/photo-1523275335684-37898b6baf30">
<h3>Smart Watch</h3>
<p>₹3,999</p>
<button>Buy Now</button>
</div>

<div class="product-card">
<img src="https://images.unsplash.com/photo-1511707171634-5f897ff02aa9">
<h3>Smart Phone</h3>
<p>₹24,999</p>
<button>Buy Now</button>
</div>

<div class="product-card">
<img src="https://images.unsplash.com/photo-1585386959984-a4155224a1ad">
<h3>Wireless Headphones</h3>
<p>₹2,499</p>
<button>Buy Now</button>
</div>

<div class="product-card">
<img src="https://images.unsplash.com/photo-1526170375885-4d8ecf77b99f">
<h3>Digital Camera</h3>
<p>₹35,000</p>
<button>Buy Now</button>
</div>

</div>

</section>

<!-- ABOUT -->
<section id="about" class="about">

<h2 class="section-title">About Us</h2>

<p>
Harini Store is a modern commercial platform created to provide
customers with reliable and high-quality electronic products.
Our goal is to combine technology and convenience through an easy-to-use
online shopping experience.
</p>

<p>
We carefully select products that meet international standards of
performance and durability. Our team continuously works to introduce
innovative gadgets that improve everyday living.
</p>

<p>
Why Choose Us?
</p>

<ul>
<li>✔ Affordable Prices</li>
<li>✔ Trusted Quality Products</li>
<li>✔ Fast Delivery Service</li>
<li>✔ Customer Friendly Support</li>
</ul>

</section>

<!-- CONTACT -->
<section id="contact" class="contact">

<h2 class="section-title">Contact Us</h2>

<form>
<input type="text" placeholder="Your Name" required>
<input type="email" placeholder="Email Address" required>
<textarea placeholder="Your Message"></textarea>
<button type="submit">Send Message</button>
</form>

</section>

<!-- FOOTER -->
<footer>
<p>© 2026 Harini Store | All Rights Reserved</p>
</footer>

</body>
</html>
```

## style.css

```
/* RESET */
*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:Arial, sans-serif;
scroll-behavior:smooth;
}

/* NAVBAR */
.navbar{
display:flex;
justify-content:space-between;
align-items:center;
background:#222;
color:white;
padding:15px 40px;
position:sticky;
top:0;
}

.navbar nav a{
color:white;
text-decoration:none;
margin-left:20px;
font-weight:bold;
}

.navbar nav a:hover{
color:#ff9800;
}

/* SECTION COMMON */
section{
padding:80px 40px;
min-height:100vh;
}

.section-title{
text-align:center;
margin-bottom:30px;
font-size:30px;
}

/* HOME */
.home{
background:#f5f5f5;
display:flex;
justify-content:center;
align-items:center;
text-align:center;
}

.home-content{
max-width:700px;
}

.home h1{
font-size:40px;
margin-bottom:20px;
}

.home p{
margin-bottom:15px;
line-height:1.6;
}

.btn{
display:inline-block;
margin-top:20px;
padding:12px 25px;
background:#ff9800;
color:white;
text-decoration:none;
border-radius:5px;
}

/* PRODUCTS */
.products{
display:flex;
flex-wrap:wrap;
justify-content:center;
gap:25px;
}

.product-card{
width:250px;
background:white;
border-radius:10px;
overflow:hidden;
box-shadow:0 4px 10px rgba(0,0,0,0.2);
text-align:center;
display:flex;
flex-direction:column;
}

.product-card img{
width:100%;
height:200px;
object-fit:cover;
}

.product-card h3{
margin:10px;
}

.product-card p{
color:#ff5722;
font-weight:bold;
}

.product-card button{
margin:15px;
padding:10px;
border:none;
background:#ff9800;
color:white;
cursor:pointer;
border-radius:5px;
}

.product-card button:hover{
background:#e68900;
}

/* ABOUT */
.about{
background:#fafafa;
text-align:center;
}

.about p{
max-width:800px;
margin:auto;
margin-bottom:15px;
line-height:1.7;
}

.about ul{
list-style:none;
margin-top:20px;
}

/* CONTACT */
.contact{
background:#f0f0f0;
text-align:center;
}

form{
max-width:400px;
margin:auto;
display:flex;
flex-direction:column;
gap:10px;
}

input, textarea{
padding:10px;
border-radius:5px;
border:1px solid #ccc;
}

button{
background:#222;
color:white;
padding:10px;
border:none;
cursor:pointer;
}

/* FOOTER */
footer{
background:#222;
color:white;
text-align:center;
padding:20px;
}

/* RESPONSIVE */
@media(max-width:768px){

.navbar{
flex-direction:column;
gap:10px;
}

.products{
flex-direction:column;
align-items:center;
}

}

```


## OUTPUT

<img width="1883" height="877" alt="image" src="https://github.com/user-attachments/assets/b71b4f9b-c1f2-4351-b532-373bc46a9bda" />
<img width="1871" height="904" alt="image" src="https://github.com/user-attachments/assets/13180107-bac9-4a13-a31c-7d5e19b39d51" />
<img width="1891" height="907" alt="image" src="https://github.com/user-attachments/assets/28964774-13ce-41fe-ad0f-204502ca5191" />
<img width="1871" height="901" alt="image" src="https://github.com/user-attachments/assets/91b80e17-1d30-48b2-89c6-57114e964b3c" />

## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
