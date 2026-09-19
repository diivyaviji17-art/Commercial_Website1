# Ex02 Commercial Website
## Date:

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
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>NexaMart</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <!-- Navigation -->
    <nav>
        <h1>🛒 NexaMart</h1>

        <ul>
            <li><a href="#">Home</a></li>
            <li><a href="#products">Products</a></li>
            <li><a href="#">Offers</a></li>
            <li><a href="#creator">Creator</a></li>
        </ul>
    </nav>

    <!-- Hero Section -->
    <section class="hero">

        <div class="hero-text">
            <h2><h2>🛒 Everything You Need, All in One Place!</h2></h2>

            <p>
                Everything you need, all in one place! Explore the latest fashion,
                electronics, accessories, and everyday essentials at amazing prices.
                Shop smarter with NovaMart.
            </p>

            <button>Shop Now</button>

        </div>

        <div class="hero-image">
            <img src="sale.avif">
        </div>

    </section>

    <!-- Products -->

    <section class="products" id="products">

        <h2>🌟 Featured Products 🌟</h2>

        <div class="product-container">

            <div class="card">
                <img src="shoe.jpg">

                <h3>Sports Shoes</h3>

                <p>Comfortable running shoes.</p>

                <h4>₹4,999</h4>

                <button>Buy Now</button>

            </div>

            <div class="card">

                <img src="phone.jpg">

                <h3>Smart Phone</h3>

                <p>Latest flagship smartphone.</p>

                <h4>₹49,999</h4>

                <button>Buy Now</button>

            </div>

            <div class="card">

                <img src="Headphone.jpg">

                <h3>Wireless Headphones</h3>

                <p>Crystal clear sound quality.</p>

                <h4>₹3,499</h4>

                <button>Buy Now</button>

            </div>

            <div class="card">

                <img src="tshirt.jpg">

                <h3>Fashion T-Shirt</h3>

                <p>Premium cotton casual wear.</p>

                <h4>₹999</h4>

                <button>Buy Now</button>

            </div>

        </div>

    </section>

    <!-- Creator -->

    <section class="creator" id="creator">

        <div class="creator-card">

            <img src="image.jpg">
            <h2>R.Divyadharshini 💜</h2>

            <p class="tagline">
                ✨ Web Designer | Creative Thinker | Future Software Engineer ✨
            </p>

            <p>📧 diivyaviji17@gmail.com</p>

            <p>
                💼
                <a href="https://www.linkedin.com/in/r-divyadharshini-raja-627417380" target="_blank">
                    Visit My LinkedIn
                </a>
            </p>

            <p class="thanks">
                💖 Thank you for visiting NexaMart! 💖
            </p>

        </div>

    </section>

    <!-- Footer -->

    <footer>

        <p>© 2026 NexaMart | Designed with ❤️ by <b>R.Divyadharshini</b></p>

    </footer>

</body>
</html>
```
style.css
```
```css
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:Arial, Helvetica, sans-serif;
}

body{
    background:linear-gradient(135deg,#f4f7fc,#dbeafe);
}

/* Navigation */

nav{
    display:flex;
    justify-content:space-between;
    align-items:center;
    background:linear-gradient(to right,#1e3a8a,#2563eb);
    padding:20px 60px;
    position:sticky;
    top:0;
}

nav h1{
    color:white;
    font-size:34px;
}

nav ul{
    display:flex;
    list-style:none;
}

nav ul li{
    margin-left:30px;
}

nav ul li a{
    color:white;
    text-decoration:none;
    font-size:18px;
    transition:.3s;
}

nav ul li a:hover{
    color:#cbd5e1;
}

/* Hero */

.hero{
    display:flex;
    justify-content:space-around;
    align-items:center;
    flex-wrap:wrap;
    padding:70px;
}

.hero-text{
    width:45%;
}

.hero-text h2{
    color:#1e3a8a;
    font-size:48px;
    margin-bottom:20px;
}

.hero-text p{
    color:#374151;
    font-size:20px;
    line-height:1.6;
    margin-bottom:25px;
}

.hero button{
    background:#2563eb;
    color:white;
    border:none;
    padding:15px 35px;
    border-radius:30px;
    cursor:pointer;
    font-size:18px;
    transition:.3s;
}

.hero button:hover{
    background:#1e40af;
}

.hero-image img{
    width:420px;
    border-radius:20px;
    box-shadow:0 10px 20px rgba(0,0,0,.2);
}

/* Products */

.products{
    text-align:center;
    padding:60px;
}

.products h2{
    color:#1e3a8a;
    font-size:40px;
    margin-bottom:35px;
}

.product-container{
    display:flex;
    justify-content:center;
    flex-wrap:wrap;
    gap:30px;
}

.card{
    width:260px;
    background:white;
    border-radius:20px;
    overflow:hidden;
    box-shadow:0 8px 16px rgba(0,0,0,.15);
    transition:.4s;
}

.card:hover{
    transform:translateY(-10px);
}

.card img{
    width:100%;
    height:220px;
    object-fit:cover;
}

.card h3{
    color:#1e3a8a;
    margin:15px;
}

.card p{
    color:#555;
    margin:10px;
}

.card h4{
    color:#2563eb;
    margin:10px;
    font-size:24px;
}

.card button{
    background:#2563eb;
    color:white;
    border:none;
    padding:12px 25px;
    border-radius:30px;
    margin-bottom:20px;
    cursor:pointer;
    transition:.3s;
}

.card button:hover{
    background:#1e40af;
}

/* Creator */

.creator{
    display:flex;
    justify-content:center;
    padding:60px 20px;
}

.creator-card{
    width:380px;
    background:linear-gradient(135deg,#ffffff,#e5e7eb);
    padding:30px;
    border-radius:25px;
    text-align:center;
    box-shadow:0 10px 20px rgba(0,0,0,.15);
    transition:.4s;
}

.creator-card:hover{
    transform:scale(1.03);
}

.creator-card img{
    width:120px;
    height:120px;
    border-radius:50%;
    border:5px solid white;
    margin-bottom:15px;
}

.creator-card h2{
    color:#1e3a8a;
    margin-bottom:10px;
}

.tagline{
    color:#4b5563;
    font-style:italic;
    margin-bottom:20px;
}

.creator-card p{
    margin:12px 0;
    font-size:17px;
    color:#374151;
}

.creator-card a{
    color:#2563eb;
    text-decoration:none;
    font-weight:bold;
}

.creator-card a:hover{
    color:#1e40af;
}

.thanks{
    color:#1e3a8a;
    font-weight:bold;
    margin-top:20px;
}

/* Footer */

footer{
    background:#111827;
    color:white;
    text-align:center;
    padding:20px;
    margin-top:30px;
}

/* Responsive */

@media(max-width:768px){

    nav{
        flex-direction:column;
    }

    nav ul{
        margin-top:15px;
    }

    .hero{
        flex-direction:column;
        text-align:center;
    }

    .hero-text{
        width:100%;
        margin-bottom:30px;
    }

    .hero-image img{
        width:90%;
    }
}
```
## OUTPUT
<img width="1917" height="915" alt="Screenshot 2026-09-19 213321" src="https://github.com/user-attachments/assets/07795434-3bef-426d-94e6-69b4b3468a9e" />
<img width="1905" height="911" alt="Screenshot 2026-09-19 213330" src="https://github.com/user-attachments/assets/a152025c-f26e-4fb6-bdab-1f39ca3a7e93" />
<img width="1906" height="898" alt="Screenshot 2026-09-19 213339" src="https://github.com/user-attachments/assets/6bd1929b-af9d-4245-bf2c-40f2b177e6ba" />




## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
