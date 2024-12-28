
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
.button {
    display: inline-block;
    padding: 10px 20px;
    font-size: 16px;
    color: white;
    background-color: #4caf50;
    text-decoration: none;
    border-radius: 4px;
    cursor: pointer;
}

.button:hover {
    background-color: #45a049;
}
</style>
<body>
    <!-- Header Section -->
    <header>
        <div class="logo">
            <img src="galogo.jpg"  />
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
            <a href="cer.html" class="button">Shop Now</button>
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
