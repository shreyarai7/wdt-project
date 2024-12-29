
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GreenAura Shopping</title>
    <style>
        /* Global Reset */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        /* Body Styling */
        body {
            font-family: 'Arial', sans-serif;
            line-height: 1.6;
            color: #333;
            background: #f4f4f4;
            margin: 0;
            padding: 0;
        }

        /* Header Section */
        header {
            background: #2d6a4f;
            color: white;
            padding: 10px 20px;
            text-align: center;
        }

        header h1 {
            font-size: 1.8em;
        }

        nav {
            display: flex;
            justify-content: center;
            background: #1b4332;
            padding: 10px;
        }

        nav a {
            color: white;
            text-decoration: none;
            margin: 0 15px;
            font-size: 1.1em;
        }

        nav a:hover {
            text-decoration: underline;
        }

        /* Main Section */
        main {
            max-width: 960px;
            margin: 20px auto;
            padding: 10px;
        }

        .hero {
            background: #95d5b2;
            text-align: center;
            padding: 20px;
            border-radius: 10px;
            margin-bottom: 20px;
        }

        .hero h2 {
            font-size: 1.8em;
            margin-bottom: 10px;
        }

        .hero p {
            margin-bottom: 15px;
            font-size: 1.2em;
        }

        .hero button {
            padding: 10px 20px;
            font-size: 1em;
            background: #1b4332;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }

        .hero button:hover {
            background: #081c15;
        }

        /* Search Section */
        .search-block {
            margin: 20px 0;
            text-align: center;
        }

        .search-block input {
            padding: 10px;
            font-size: 1em;
            width: 70%;
            max-width: 500px;
            border: 1px solid #ccc;
            border-radius: 5px;
        }

        .search-block button {
            padding: 10px 20px;
            background: #2d6a4f;
            color: white;
            border: none;
            font-size: 1em;
            border-radius: 5px;
            cursor: pointer;
        }

        .search-block button:hover {
            background: #1b4332;
        }

        /* Product Grid */
        .product-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
            gap: 15px;
        }

        .product-card {
            background: white;
            border: 1px solid #ddd;
            border-radius: 5px;
            overflow: hidden;
            text-align: center;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
        }

        .product-card img {
            width: 100%;
            height: 150px;
            object-fit: cover;
        }

        .product-card h3 {
            font-size: 1.2em;
            margin: 10px 0;
        }

        .product-card p {
            font-size: 0.9em;
            margin: 5px 10px;
        }

        .product-card a {
            display: block;
            padding: 10px;
            background: #2d6a4f;
            color: white;
            text-decoration: none;
            border-radius: 0 0 5px 5px;
        }

        .product-card a:hover {
            background: #1b4332;
        }

        /* Footer Section */
        footer {
            background: #2d6a4f;
            color: white;
            text-align: center;
            padding: 10px 20px;
            margin-top: 20px;
        }

        footer p {
            font-size: 0.9em;
        }

        footer a {
            color: #f39c12;
            text-decoration: none;
        }

        footer a:hover {
            text-decoration: underline;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            header h1 {
                font-size: 1.5em;
            }

            .hero h2 {
                font-size: 1.5em;
            }

            nav a {
                font-size: 0.9em;
                margin: 0 8px;
            }
        }
        /* Responsive Design */
@
}
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <div class="logo">
            <img src="galogo1.jpg"  /> </div>
        <h1>Welcome to GreenAura</h1>
    </header>

    <!-- Navigation -->
    <nav>
        <a href="popo.html">Home</a>
        <a href ="cer.html">products</a>
        <a href="about.html">About</a>
        <a href="login.html">Login</a>
      
    </nav>

    <!-- Main Section -->
    <main>
        <!-- Hero Section -->
        <section class="hero">
            <h2>Discover Your Green Haven</h2>
            <p>Your one-stop destination for plants, pots, and more.</p>
            <button id="shop-now">Shop Now</button>
        </section>

        <!-- Search Section -->
        <div class="search-block">
            <input type="text" id="search-bar" placeholder="Search for products...">
            <button id="search-button">Search</button>
        </div>

        <!-- Product Section -->
        <section class="product-grid">
            <div class="product-card">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQNUN6DTUg9burPhFIU4Y8D-9Hy2_IYcE-DJw&s" alt="Indoor Plant">
                <h3>Indoor Plant</h3>
                <p>Perfect for adding life to your home.</p>
                <a href="cer.html">View Product</a>
            </div>
            <div class="product-card">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQzX-5OQNI1jLQAydkjHEu3abhdcuZTbT4dJQ&s" alt="Outdoor Plant">
                <h3>Outdoor Plant</h3>
                <p>Ideal for your garden or balcony.</p>
                <a href="cer.html">View Product</a>
            </div>
            <div class="product-card">
                <img src="https://encrypted-tbn0.gstatic.com/shopping?q=tbn:ANd9GcTbmgYWA1ahAydNumSgaxb8a-02XFyo_2sbbkQsAkV8aV9immfi91ILmW7bslIwALmRrnyWiclrfaOohWZp9vg5_lbJq0v6nqU1GkMza2m6" alt="Cactus">
                <h3>Cactus</h3>
                <p>Low-maintenance and stylish.</p>
                <a href="cer.html">View Product</a>
            </div>
        </section>
    </main>

    <!-- Footer -->
    <footer>
        <p>© 2024 GreenAura. All Rights Reserved. | <a href="cer.html">Shop Now</a></p>
    </footer>

    <!-- JavaScript -->
    <script>
        // Shop Now Button Alert
        document.getElementById('shop-now').addEventListener('click', function () {
            alert('Redirecting to our product page!');
            location.href = 'cer.html';
        });

        // Search Functionality
        document.getElementById('search-button').addEventListener('click', function () {
            const query = document.getElementById('shop-now').value.toLowerCase();
            const products = document.querySelectorAll('product-card');

            products.forEach(product => {
                const title = product.querySelector('h3').textContent.toLowerCase();
                if (title.includes(query)) {
                    product.style.display = 'block';
                } else {
                    product.style.display = 'none';
                }
            });
        });
    </script>
    <script>
    function showLoginPrompt() {
        // Show a custom alert box with a message asking user to login
        const isLoginConfirmed = confirm("You need to log in to make a purchase or view your cart. Would you like to go to the login page?");
        if (isLoginConfirmed) {
            // If user clicks OK, redirect to the login page
            window.location.href = 'login.html';
        }
    }

    // Function to attach event listeners to buttons and product cart div
    function attachLoginPrompt() {
        const buyNowButton = document.getElementById('shop-now'); // Button to Buy Now
        const addToCartButton = document.getElementById('product-cards'); // Button to Add to Cart
        const productCart = document.getElementById('productCart'); // Div for the product cart

        // Attach event listener to the "Buy Now" button
        if (buyNowButton) {
            buyNowButton.addEventListener('click', function(event) {
                event.preventDefault(); // Prevent the default action of the button (navigation)
                showLoginPrompt(); // Show login prompt
            });
        }

        // Attach event listener to the "Add to Cart" button
        if (addToCartButton) {
            addToCartButton.addEventListener('click', function(event) {
                event.preventDefault(); // Prevent the default action (adding item to cart)
                showLoginPrompt(); // Show login prompt
            });
        }

        // Attach event listener to the "productCart" div (if user interacts with the product cart)
        if (productCart) {
            productCart.addEventListener('click', function(event) {
                event.preventDefault(); // Prevent default behavior (viewing cart or navigating)
                showLoginPrompt(); // Show login prompt
            });
        }
    }

    // Attach login prompt functionality when the page loads
    window.onload = function() {
        attachLoginPrompt();
    };
</script>
    
</body>
</html>
