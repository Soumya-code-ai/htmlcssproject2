html code-->
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Neighborhood Cafe</title>
  <link rel="stylesheet" href="mstyle.css">
</head>
<body>

  <!-- Navigation -->
  <nav class="nav">
    <div class="brand">
      <div class="logo">NB</div>
      <div>
        <h1>Neighborhood Cafe</h1>
        <p>Open • 7:00 AM - 9:00 PM</p>
      </div>
    </div>
    <ul class="nav-links">
      <li><a href="#services">Services</a></li>
      <li><a href="#about">About</a></li>
      <li><a href="#contact">Contact</a></li>
      <li><button class="cta">Order Now</button></li>
    </ul>
  </nav>

  <!-- Hero -->
  <header class="hero">
    <div class="hero-text">
      <h2>Warm brews, fresh bites — right in your neighbourhood</h2>
      <p>Your cozy corner for specialty coffee, homemade sandwiches, and friendly faces.</p>
      <div class="features">
        <span>Free Wi-Fi</span>
        <span>Locally sourced</span>
        <span>Outdoor seating</span>
      </div>
    </div>
  </header>

  <!-- Services -->
  <section id="services" class="services">
    <h2>Our Services</h2>
    <div class="service-list">
      <div class="service">
        <h3>☕ Specialty Coffee</h3>
        <p>Single origin beans, skilled baristas.</p>
      </div>
      <div class="service">
        <h3>🥪 Fresh Sandwiches</h3>
        <p>Daily-baked bread & seasonal fillings.</p>
      </div>
      <div class="service">
        <h3>🎂 Homemade Desserts</h3>
        <p>Ask about today's specials.</p>
      </div>
    </div>
  </section>

  <!-- About + Contact -->
  <section id="about" class="about-contact">
    <div class="about">
      <h2>About Us</h2>
      <p>Started by locals with a love for coffee and conversation. We believe in friendly service and building community — one cup at a time.</p>
    </div>
    <div id="contact" class="contact-form">
      <h2>Contact Us</h2>
      <form>
        <input type="text" placeholder="Your Name" required>
        <input type="text" placeholder="Phone or Email" required>
        <textarea placeholder="Message" rows="4"></textarea>
        <button type="submit">Send Message</button>
      </form>
    </div>
  </section>

  <!-- Footer -->
  <footer>
    <p>© <span id="year"></span> Neighborhood Cafe — Made with ☕</p>
  </footer>

  <script>
    document.getElementById('year').textContent = new Date().getFullYear();
  </script>

</body>
</html>
external css-->
:root {
  --bg: #f7f7f9;
  --card: #fff;
  --accent: #d97706;
  --muted: #666768;
}

body {
  font-family: Arial, sans-serif;
  margin: 0;
  background: var(--bg);
  color: #111;
}

/* Navigation */
.nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background: white;
  padding: 10px 20px;
  box-shadow: 0 4px 10px rgba(0,0,0,0.05);
}

.brand {
  display: flex;
  align-items: center;
  gap: 10px;
}

.logo {
  background: var(--accent);
  color: white;
  padding: 10px;
  border-radius: 8px;
  font-weight: bold;
}

.nav-links {
  display: flex;
  gap: 15px;
  list-style: none;
}

.nav-links a {
  text-decoration: none;
  color: var(--muted);
  font-weight: bold;
}

.cta {
  background: var(--accent);
  color: white;
  border: none;
  padding: 8px 12px;
  border-radius: 6px;
  cursor: pointer;
}

/* Hero */
.hero {
  padding: 40px 20px;
  text-align: center;
  background: #fff3e0;
}

.features span {
  background: var(--accent);
  color: white;
  padding: 5px 10px;
  margin: 5px;
  border-radius: 20px;
  font-size: 0.9rem;
  display: inline-block;
}

/* Services */
.services {
  padding: 30px 20px;
  text-align: center;
}

.service-list {
  display: flex;
  gap: 15px;
  flex-wrap: wrap;
  justify-content: center;
}

.service {
  background: var(--card);
  padding: 15px;
  border-radius: 8px;
  width: 250px;
  box-shadow: 0 4px 10px rgba(0,0,0,0.05);
}

/* About + Contact */
.about-contact {
  display: flex;
  gap: 20px;
  padding: 30px 20px;
  flex-wrap: wrap;
}

.about, .contact-form {
  flex: 1;
  min-width: 280px;
  background: var(--card);
  padding: 15px;
  border-radius: 8px;
  box-shadow: 0 4px 10px rgba(0,0,0,0.05);
}

.contact-form input, .contact-form textarea, .contact-form button {
  width: 100%;
  padding: 8px;
  margin-top: 8px;
  border: 1px solid #ccc;
  border-radius: 6px;
}

.contact-form button {
  background: var(--accent);
  color: white;
  border: none;
  cursor: pointer;
}

/* Footer */
footer {
  text-align: center;
  padding: 15px;
  color: var(--muted);
  font-size: 0.9rem;
}
