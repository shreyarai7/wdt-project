

<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>GreenAura</title>
  <link rel="stylesheet" href="styles.css">
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&display=swap" rel="stylesheet">
  <script defer src="script.js"></script>
</head>
<style>
    /* General Reset */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: 'Poppins', sans-serif;
  line-height: 1.6;
  background: #f0f8f4;
  color: #333;
  scroll-behavior: smooth;
}

/* Navbar */
.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1rem 2rem;
  background: linear-gradient(90deg, #004d40, #00796b);
  position: sticky;
  top: 0;
  z-index: 1000;
}

.logo {
  width: 140px;
}

.nav-links {
  list-style: none;
  display: flex;
}

.nav-links li {
  margin-left: 20px;
}

.nav-links a {
  color: #fff;
  text-decoration: none;
  font-weight: 600;
}

.menu-toggle {
  display: none;
  font-size: 1.5rem;
  background: none;
  border: none;
  color: #fff;
}

@media (max-width: 768px) {
  .menu-toggle {
    display: block;
  }

  .nav-links {
    display: none;
    flex-direction: column;
    background: #004d40;
    position: absolute;
    right: 0;
    top: 60px;
    width: 200px;
  }

  .nav-links.active {
    display: flex;
  }
}

/* Hero Section */
.hero {
  height: 100vh;
  background: linear-gradient(to right, #b9fbc0, #00c853);
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  color: #fff;
}

.hero h1 {
  font-size: 3rem;
}

.hero .highlight {
  color: #ffcc80;
}

.hero .btn {
  margin-top: 1.5rem;
  padding: 0.8rem 1.5rem;
  background: #00796b;
  color: #fff;
  border: none;
  border-radius: 5px;
  font-size: 1rem;
  cursor: pointer;
  text-decoration: none;
}

.hero .btn:hover {
  background: #004d40;
}

/* About Section */
.about {
  padding: 4rem 2rem;
  text-align: center;
  background: #f9fbe7;
}

/* Services Section */
.services {
  padding: 4rem 2rem;
  text-align: center;
}

.service-cards {
  display: flex;
  justify-content: center;
  gap: 2rem;
}

.card {
  background: #fff;
  padding: 2rem;
  border-radius: 10px;
  box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
  width: 300px;
  text-align: center;
}

/* Contact Section */
.contact {
  padding: 4rem 2rem;
  text-align: center;
}

.contact-form input,
.contact-form textarea {
  width: 100%;
  padding: 1rem;
  margin-bottom: 1rem;
  border: 1px solid #ccc;
  border-radius: 5px;
}

.contact-form .btn {
  background: #00796b;
  color: #fff;
}

/* Footer */
footer {
  padding: 1rem;
  text-align: center;
  background: #004d40;
  color: #fff;
}

/* Scroll-to-Top Button */
#scrollToTop {
  position: fixed;
  bottom: 20px;
  right: 20px;
  background: #00796b;
  color: #fff;
  border: none;
  border-radius: 50%;
  font-size: 1.5rem;
  padding: 0.8rem;
  display: none;
  cursor: pointer;
}

#scrollToTop:hover {
  background: #004d40;
}
</style>
<body>
  <!-- Navbar -->
  <header>
    <nav class="navbar">
      <img src="galogo.jpg" alt="GreenAura Logo" class="logo">
      <button class="menu-toggle" aria-label="Toggle navigation">☰</button>
      <ul class="nav-links">
        <li><a href="popo.html">Home</a></li>
        <li><a href="about.html">About</a></li>
        <li><a href="cer.html">products</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </header>

  <!-- Hero Section -->
  <section id="home" class="hero">
    <div class="hero-content">
      <h1>Welcome to <span class="highlight">GreenAura</span></h1>
      <p>Discover the beauty of sustainability and transform the world with eco-friendly choices.</p>
      <a href="about.html" class="btn">Learn More</a>
    </div>
  </section>

  <!-- About Section -->
  <section id="about" class="about">
    <h2>About Us</h2>
    <p>GreenAura is dedicated to promoting sustainable living through eco-friendly solutions. Join us on this journey to a greener future.</p>
  </section>

  <!-- Services Section -->
  <section id="services" class="services">
    <h2>Our Services</h2>
    <div class="service-cards">
      <div class="card">
        <h3>Eco Products</h3>
        <p>High-quality products that are kind to the planet.</p>
      </div>
      <div class="card">
        <h3>Consulting</h3>
        <p>Expert advice on sustainability for businesses and individuals.</p>
      </div>
      <div class="card">
        <h3>Workshops</h3>
        <p>Interactive sessions to teach eco-friendly practices.</p>
      </div>
    </div>
  </section>

  <!-- Contact Section -->
  <section id="contact" class="contact">
    <h2>Contact Us</h2>
    <form class="contact-form">
      <input type="text" placeholder="Your Name" required>
      <input type="email" placeholder="Your Email" required>
      <textarea placeholder="Your Message" rows="5" required></textarea>
      <button type="submit" class="btn">Send Message</button>
    </form>
  </section>

  <!-- Footer -->
  <footer>
    <p>&copy; 2024 GreenAura | Designed with ❤ for sustainability.</p>
  </footer>

  <!-- Scroll-to-Top Button -->
  <button id="scrollToTop" aria-label="Scroll to top">↑</button>
<script>
    // Navbar Toggle
const menuToggle = document.querySelector('.menu-toggle');
const navLinks = document.querySelector('.nav-links');

menuToggle.addEventListener('click', () => {
  navLinks.classList.toggle('active');
});

// Scroll-to-Top Button
const scrollToTopButton = document.getElementById('scrollToTop');

window.addEventListener('scroll', () => {
  if (window.scrollY > 300) {
    scrollToTopButton.style.display = 'block';
  } else {
    scrollToTopButton.style.display = 'none';
  }
});

scrollToTopButton.addEventListener('click', () => {
  window.scrollTo({ top: 0, behavior: 'smooth' });
});
</script>
</body>
</html>
