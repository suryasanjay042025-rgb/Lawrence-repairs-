# Lawrence-repairs-<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Lawrence Computer & Printer Repairs</title>

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: Arial, sans-serif;
}

body {
    line-height: 1.6;
}

/* Header */
header {
    background: #0d47a1;
    color: white;
    padding: 15px 0;
    text-align: center;
}

header h1 {
    margin-bottom: 5px;
}

/* Navigation */
nav {
    background: #1565c0;
    display: flex;
    justify-content: center;
    padding: 10px;
}

nav a {
    color: white;
    margin: 0 15px;
    text-decoration: none;
    font-weight: bold;
}

nav a:hover {
    text-decoration: underline;
}

/* Hero Section */
.hero {
    background: url('https://images.unsplash.com/photo-1581092160562-40aa08e78837') no-repeat center/cover;
    color: white;
    padding: 100px 20px;
    text-align: center;
}

.hero h2 {
    font-size: 40px;
}

.hero p {
    margin: 15px 0;
    font-size: 18px;
}

.hero button {
    padding: 10px 20px;
    background: #ff9800;
    border: none;
    color: white;
    cursor: pointer;
    font-size: 16px;
}

/* Sections */
section {
    padding: 40px 20px;
    text-align: center;
}

/* Services */
.services {
    background: #f4f4f4;
}

.service-box {
    display: inline-block;
    width: 250px;
    margin: 15px;
    padding: 20px;
    background: white;
    border-radius: 10px;
    box-shadow: 0 0 10px rgba(0,0,0,0.1);
}

/* Contact */
.contact form {
    max-width: 400px;
    margin: auto;
}

.contact input, .contact textarea {
    width: 100%;
    padding: 10px;
    margin: 10px 0;
}

.contact button {
    padding: 10px;
    background: #0d47a1;
    color: white;
    border: none;
    cursor: pointer;
}

/* Footer */
footer {
    background: #0d47a1;
    color: white;
    text-align: center;
    padding: 15px;
}

/* Floating Buttons */
.whatsapp, .call {
    position: fixed;
    right: 20px;
    padding: 12px;
    color: white;
    border-radius: 50%;
    text-align: center;
}

.whatsapp {
    bottom: 80px;
    background: #25D366;
}

.call {
    bottom: 20px;
    background: #2196f3;
}

/* Responsive */
@media(max-width: 768px) {
    .service-box {
        width: 90%;
    }
}
</style>
</head>

<body>

<header>
    <h1>Lawrence Computer & Printer Repairs</h1>
    <p>Fast & Reliable Repair Services</p>
</header>

<nav>
    <a href="#home">Home</a>
    <a href="#services">Services</a>
    <a href="#about">About</a>
    <a href="#contact">Contact</a>
</nav>

<section class="hero" id="home">
    <h2>Your Tech, Our Responsibility</h2>
    <p>Expert repair for computers, laptops, and printers</p>
    <button onclick="scrollToContact()">Contact Now</button>
</section>

<section class="services" id="services">
    <h2>Our Services</h2>

    <div class="service-box">
        <h3>Computer Repair</h3>
        <p>Hardware & software troubleshooting</p>
    </div>

    <div class="service-box">
        <h3>Laptop Repair</h3>
        <p>Screen, battery, motherboard fixes</p>
    </div>

    <div class="service-box">
        <h3>Printer Repair</h3>
        <p>All brands serviced quickly</p>
    </div>

    <div class="service-box">
        <h3>Virus Removal</h3>
        <p>Keep your system safe & secure</p>
    </div>

</section>

<section id="about">
    <h2>About Us</h2>
    <p>
        Lawrence Computer & Printer Repairs provides professional and affordable
        repair services. We specialize in quick diagnostics and reliable solutions
        to get your devices back to working condition.
    </p>
</section>

<section class="contact" id="contact">
    <h2>Contact Us</h2>

    <form onsubmit="submitForm(event)">
        <input type="text" placeholder="Your Name" required>
        <input type="email" placeholder="Your Email" required>
        <textarea rows="5" placeholder="Your Message"></textarea>
        <button type="submit">Send Message</button>
    </form>

</section>

<footer>
    <p>© 2026 Lawrence Computer & Printer Repairs</p>
</footer>

<!-- Floating Buttons -->
<a href="https://wa.me/your-number" class="whatsapp">💬</a>
<a href="tel:your-number" class="call">📞</a>

<script>
function scrollToContact() {
    document.getElementById("contact").scrollIntoView({
        behavior: "smooth"
    });
}

function submitForm(e) {
    e.preventDefault();
    alert("Message sent successfully!");
}
</script>

</body>
</html>
