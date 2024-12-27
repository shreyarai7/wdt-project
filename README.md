<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="G - Your Green Companion for Plants & Gardening">
    <title>GreenAura</title>
    <link rel="stylesheet" href="style.css">
</head>
<style>
  /* General Reset */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

/* Body and Typography */
body {
    font-family: 'Arial', sans-serif;
    line-height: 1.6;
    background-color: #83b2cf;
    color: #450505;
}

h1, h2, h3 {
    color: #2c3e50;
}

p {
    margin: 10px 0;
}

/* Header Section */
header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    background-color: #329635;
    color: white;
    padding: 10px 20px;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

header .logo {
    display: flex;
    align-items: center;
}

header .logo img {
    width: 50px;
    margin-right: 10px;
}

header .logo h1 {
    font-size: 1.8rem;
}

nav ul {
    list-style: none;
    display: flex;
}

nav ul li {
    margin-left: 20px;
}

nav ul li a {
    color: rgb(57, 9, 9);
    text-decoration: none;
    font-weight: bold;
    font-size: 1rem;
}

nav ul li a:hover {
    text-decoration: underline;
}

/* Hero Section */
.hero {
    text-align: center;
    background: url('images/hero-bg.jpg') no-repeat center center/cover;
    color: rgb(117, 31, 31);
    padding: 100px 20px;
}

.hero h2 {
    font-size: 2.5rem;
    margin-bottom: 20px;
}

.hero p {
    font-size: 1.2rem;
}

.hero button {
    background-color: #4CAF50;
    color: white;
    border: none;
    padding: 10px 20px;
    cursor: pointer;
    margin-top: 20px;
    font-size: 1rem;
    border-radius: 5px;
}

.hero button:hover {
    background-color: #080e08;
}

/* Table Section */
table {
    width: 80%;
    margin: 20px auto;
    border-collapse: collapse;
    background-color: #fff;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

caption {
    font-size: 1.5rem;
    margin-bottom: 10px;
    font-weight: bold;
}

th, td {
    padding: 12px;
    text-align: center;
    border: 1px solid #ddd;
}

th {
    background-color: #4CAF50;
    color: white;
}

tr:nth-child(even) {
    background-color: #f9f9f9;
}

/* Contact Form */
form {
    width: 60%;
    margin: 20px auto;
    padding: 20px;
    background: #fff;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
    border-radius: 5px;
}

label {
    display: block;
    margin-bottom: 8px;
    font-weight: bold;
}

input, textarea {
    width: 100%;
    padding: 10px;
    margin-bottom: 15px;
    border: 1px solid #ccc;
    border-radius: 5px;
}

input:focus, textarea:focus {
    outline: none;
    border-color: #4CAF50;
}

button[type="submit"] {
    background-color: #4CAF50;
    color: white;
    border: none;
    padding: 10px 20px;
    cursor: pointer;
    font-size: 1rem;
    border-radius: 5px;
}

button[type="submit"]:hover {
    background-color: #388E3C;
}

/* Footer */
footer {
    text-align: center;
    background-color: #2c3e50;
    color: white;
    padding: 10px 0;
    margin-top: 20px;
}

/* Image Gallery Section */
#gallery {
    text-align: center;
    padding: 50px 20px;
    background-color: #e8f5e9;
}

#gallery h2 {
    font-size: 2rem;
    margin-bottom: 30px;
}

.image-gallery {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 20px;
}

.image-gallery img {
    width: 100%;
    height: auto;
    border-radius: 8px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    transition: transform 0.3s ease;
}

.image-gallery img:hover {
    transform: scale(1.05);
}

/* Mobile Responsive Design */
@media (max-width: 768px) {
    header {
        flex-direction: column;
        text-align: center;
    }

    nav ul {
        flex-direction: column;
        margin-top: 10px;
    }

    nav ul li {
        margin: 5px 0;
    }

    .hero h2 {
        font-size: 2rem;
    }

    table {
        font-size: 0.9rem;
    }

    form {
        width: 90%;
    }

    .image-gallery {
        grid-template-columns: 1fr 1fr;
    }
}

@media (max-width: 480px) {
    .hero h2 {
        font-size: 1.8rem;
    }

    .hero p {
        font-size: 1rem;
    }

    .image-gallery {
        grid-template-columns: 1fr;
    }
}
</style>
<body>
    <!-- Header Section -->
    <header>
        <div class="logo">
            <img src="data:image/jpeg;base64,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""  />
            <h1>GreenAura</h1>
        </div>
        <nav>
            <ul>
                <li><a href="#home">Home🏡</a></li>
                <li><a href="cer.html">Products</a></li>
                <li><a href="about.html">About</a></li>
                <li><a href="signup.html">sign-up</a></li>
            </ul>
        </nav>
    </header>
    
    <!-- Main Section -->
    <main>
        
        <div class="search-block">
            <label for="search-bar" class="sr-only">Search for plants</label>
            <input 
                type="text" 
                id="search-bar" 
                placeholder="Search indoor, outdoor, and exotic plants...." 
                aria-label="Search indoor, outdoor, and exotic plants" 
                required />
            <button type="submit" aria-label="Submit search">🔍</button>
        </div>
        
        <!-- Hero Section -->
        <section id="home" class="hero">
            <h2>Welcome to GreenAura</h2>
            <p>Your one-stop destination for all things green!</p>
            <button onclick="shopNow()">Shop Now</button>
        </section>

        <!-- Image Gallery Section -->
        <section id="gallery">
            <h2>Our Beautiful Plants</h2>
            <div class="image-gallery">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSLvYogr9OkNlrmLz5EBbZlgBxd5ilNQ_YLjQ&s" alt="Indoor Plant 1">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRAO-PGwtHNCcHVu8BaFfGo1XVkZ5GHMn_DvQ&s" alt="Indoor Plant 2">
                <img src="https://unlimitedgreens.com/cdn/shop/articles/Exotic_Plants_Blog.png?crop=center&height=1024&v=1693033248&width=1024" alt="Exotic Plant 1">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQuAPBzT8EuEoStDbHMDfZcSDOq3u5EY5am9Q&s" alt="Succulent Plant">
                <img src="https://m.media-amazon.com/images/I/61hcnbtyRsL._AC_UF1000,1000_QL80_.jpg" alt="Outdoor Plant 1">
            </div>
        </section>

        <!-- Products Table Section -->
        <section id="products">
            <h2>Our Products</h2>
            <table>
                <caption>Plant Categories</caption>
                <thead>
                    <tr>
                        <th>Plant Type</th>
                        <th>Price</th>
                        <th>Availability</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td>Indoor Plants</td>
                        <td>$15</td>
                        <td>In Stock</td>
                    </tr>
                    <tr>
                        <td>Succulents</td>
                        <td>$10</td>
                        <td>Limited</td>
                    </tr>
                    <tr>
                        <td>Herbs</td>
                        <td>$8</td>
                        <td>In Stock</td>
                    </tr>
                </tbody>
            </table>
        </section>
        <div class="product-images">
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcR0CyZ80ChIXohalcE-kPyN7qinifk85H7muw&s" alt="Indoor Plants" style="width: 300px; margin: 20px;">
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQwYI1YSkuxwMqhLXF367Ip1amze3JBmFdEAg&s" alt="Succulents" style="width: 300px; margin: 20px;">
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTi7g2MH01Yvl3hw6FnZgweVbubOGzkQuhJuA&s" alt="Herbs" style="width: 300px; margin: 20px;">
        </div>
    </section>
    
    <!-- About Section -->
     
   
    <section id="about">
        <h2>About GreenAura....</h2>
        <style>body  {
            font-family: Verdana, sans-serif;
            font-size: 16px;
          }
          
          h2 {
            font-family: Georgia, serif;
            font-size: 46px;  
          }
            p.b{
               font: italic small-caps bold 25px/30px Georgia, serif;
             }
          </style>
        <p class="b">At Leafy Island, we believe in the beauty and tranquility that plants bring to our lives. Our mission is to offer a variety of plants for all types of environments, from cozy indoor spaces to vibrant outdoor gardens.</p>
        <div class="about-images">
            <!-- Added Image in About Section -->
            <img src=https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ_MQWzCKj6VI37Jbx7dc_ED_ZzMhDAoGgsQw&s"" alt="About Leafy Island" style="width: 300px; margin-top: 20px;">
        </div>
    </section>
    
    
        <!-- Contact Form Section -->
        <section id="contact">
            <h2>Contact Us</h2>
            <form>
                <label for="name">Name:</label>
                <input type="text" id="name" name="name" placeholder="Enter your name" required />

                <label for="email">Email:</label>
                <input type="email" id="email" name="email" placeholder="Enter your email" required />

                <label for="mobile no.">Mobile number:</label>
                <textarea id="message" name="message" rows="1" placeholder="Your number"></textarea>

                <button type="submit">Submit</button>
            </form>
        </section>
    </main>

    <!-- Footer -->
    <footer>
        <p>&copy; 2024 Leafy Island | Designed for Plant Lovers</p>
    </footer>

    <!-- JavaScript -->
    <script src="script.js">// Smooth Scroll for Navigation
        document.querySelectorAll('nav ul li a').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
        
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });
        
        // Hero Section Button Click (Scroll to Product Section)
        function shopNow() {
            document.querySelector('#products').scrollIntoView({
                behavior: 'smooth'
            });
        }
        
        // Search Feature (Dummy suggestion function)
        const searchInput = document.getElementById('search-bar');
        const searchButton = document.querySelector('.search-block button');
        
        searchButton.addEventListener('click', function() {
            let query = searchInput.value.toLowerCase();
            if(query === '') {
                alert('Please enter a search query!');
            } else {
                alert('Searching for: ' + query);
            }
        });
        
        // Image Hover Effect for Zoom
        const images = document.querySelectorAll('.image-gallery img');
        images.forEach(img => {
            img.addEventListener('mouseover', function() {
                this.style.transform = 'scale(1.1)';
            });
        
            img.addEventListener('mouseout', function() {
                this.style.transform = 'scale(1)';
            });
        });</script>
</body>
</html>
