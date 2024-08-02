<template>
  <div class="sacco-page">
    <header class="header">
      <nav class="navbar">
        <ul>
          <li><a href="#home">Home</a></li>
          <li><a href="#about">About Us</a></li>
          <li><a href="#services">Services</a></li>
          <li><a href="#contact">Contact</a></li>
        </ul>
      </nav>
    </header>

    <section id="home" class="hero-section">
      <div class="hero-content">
        <h1>Welcome to Our SACCO</h1>
        <p>Empowering our members through financial inclusion.</p>
        <button class="cta-button">Join Us Today</button>
      </div>
    </section>

    <section id="about" class="about-section">
      <h2>About Us</h2>
      <p>
        Our SACCO has been providing financial services to our community for over
        a decade. We are committed to supporting our members' financial well-being.
      </p>
    </section>

    <section id="services" class="services-section">
      <h2>Our Services</h2>
      <div class="services">
        <div class="service">
          <h3>Loans</h3>
          <p>Flexible loan options to meet your needs.</p>
        </div>
        <div class="service">
          <h3>Savings</h3>
          <p>Secure and convenient savings plans.</p>
        </div>
        <div class="service">
          <h3>Investments</h3>
          <p>Grow your wealth with our investment options.</p>
        </div>
      </div>
    </section>

    <section id="testimonials" class="testimonials-section">
      <h2>What Our Members Say</h2>
      <div class="testimonials">
        <blockquote>
          "Joining this SACCO has been a life-changing experience. The support and
          services are top-notch!"
          <cite>— Jane Doe</cite>
        </blockquote>
        <blockquote>
          "Thanks to the loan options, I was able to start my own business. Highly
          recommend!"
          <cite>— John Smith</cite>
        </blockquote>
      </div>
    </section>

    <section id="contact" class="contact-section">
      <h2>Contact Us</h2>
      <form class="contact-form">
        <label for="name">Name</label>
        <input type="text" id="name" name="name" required />

        <label for="email">Email</label>
        <input type="email" id="email" name="email" required />

        <label for="message">Message</label>
        <textarea id="message" name="message" required></textarea>

        <button type="submit">Send Message</button>
      </form>
    </section>

    <footer class="footer">
      <p>© 2024 SACCO. All rights reserved.</p>
      <div class="social-media">
        <a href="#"><i class="fab fa-facebook"></i></a>
        <a href="#"><i class="fab fa-twitter"></i></a>
        <a href="#"><i class="fab fa-instagram"></i></a>
      </div>
    </footer>
  </div>
</template>

<script>

export default {
  name: 'SaccoPage',
};
</script>

<style scoped>
*{
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
/* Reset some default styles */
body, h1, h2, p, ul, li, a, button {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

/* General styles */
.sacco-page {
  font-family: Arial, sans-serif;
  line-height: 1.6;
  color: #333;
}

/* Header styles */
.header {
  background-color: #004080;
  color: white;
  padding: 1rem;
  position: sticky;
  top: 0;
  z-index: 1000;
}

.navbar ul {
  list-style: none;
  display: flex;
  justify-content: space-around;
}

.navbar ul li{
  /* padding: 1rem; */
}

.navbar a {
  color: white;
  text-decoration: none;
  font-size: 1.2rem;
}

.navbar a:hover {
  border-bottom: 4px solid #ff6600;
}

/* Hero section styles */
.hero-section {
  background: url('src/assets/E-commerce2.webp') no-repeat center center/cover;
  height: 60vh;
  color: white;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  padding: 0 1rem;
}

.hero-content {
  max-width: 600px;
}

.cta-button {
  background-color: #ff6600;
  border: none;
  padding: 1rem 2rem;
  color: white;
  font-size: 1rem;
  cursor: pointer;
  border-radius: 5px;
  margin-top: 1rem;
}

.cta-button:hover {
  background-color: #e65c00;
}

/* About section styles */
.about-section, .services-section, .testimonials-section, .contact-section {
  padding: 2rem 1rem;
  text-align: center;
}

.about-section p, .services-section p, .testimonials-section blockquote {
  max-width: 800px;
  margin: 0 auto;
}

/* Services section styles */
.services {
  display: flex;
  justify-content: space-around;
  flex-wrap: wrap;
}

.service {
  flex: 1;
  margin: 1rem;
  padding: 1rem;
  background-color: #f5f5f5;
  border-radius: 10px;
}

.service h3 {
  margin-bottom: 0.5rem;
}

/* Testimonials section styles */
.testimonials blockquote {
  font-style: italic;
  border-left: 5px solid #ff6600;
  padding-left: 1rem;
  margin: 1rem 0;
}

.testimonials cite {
  display: block;
  margin-top: 0.5rem;
  font-style: normal;
  color: #555;
}

/* Contact section styles */
.contact-form {
  max-width: 600px;
  margin: 0 auto;
  text-align: left;
}

.contact-form label {
  display: block;
  margin-bottom: 0.5rem;
  font-weight: bold;
}

.contact-form input, .contact-form textarea {
  width: 100%;
  padding: 0.5rem;
  margin-bottom: 1rem;
  border: 1px solid #ccc;
  border-radius: 5px;
}

.contact-form button {
  background-color: #004080;
  color: white;
  border: none;
  padding: 0.5rem 1rem;
  cursor: pointer;
  border-radius: 5px;
}

.contact-form button:hover {
  background-color: #003060;
}

/* Footer styles */
.footer {
  background-color: #f5f5f5;
  padding: 1rem;
  text-align: center;
}

.footer .social-media a {
  color: #333;
  margin: 0 0.5rem;
  font-size: 1.5rem;
}

.footer .social-media a:hover {
  color: #004080;
}
</style>
