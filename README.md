<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AJINKYA DAIRY FARM</title>
    <link rel="stylesheet" href="style.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
</head>
<body>

<!-- Header -->
<header>
    <div class="container">
        <div class="logo">AJINKYA DAIRY FARM</div>
        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#services">Services</a></li>
                <li><a href="#products">Products</a></li>
                <li><a href="#gallery">Gallery</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </div>
</header>

<!-- Hero Section -->
<section id="home" class="hero">
    <div class="container hero-content">
        <h1>Fresh Milk & Dairy Products</h1>
        <p>Delivering High-Quality Milk, Ghee, Paneer & More From Our Farm To Your Home.</p>
        <a href="#contact" class="btn">Contact Us</a>
    </div>
</section>

<!-- About Section -->
<section id="about">
    <div class="container">
        <h2>About Us</h2>
        <p>Ajinkya Dairy Farm (ADF) is a trusted dairy farm located in Agave, Ratnagiri, Maharashtra. We specialize in providing fresh milk and dairy products from healthy HF cows and Murrah buffaloes.</p>
        <div class="team-grid">
            <div class="team-member">
                <img src="images/co.jpg.jpg" alt="Founder">
                <h4>Ajinkya Bhandari</h4>
                <p>Founder & Owner</p>
            </div>
        </div>
    </div>
</section>

<!-- Services Section -->
<section id="services">
    <div class="container">
        <h2>Our Services</h2>
        <div class="services-grid">
            <div class="service-item">
                <i class="fas fa-cow"></i>
                <h3>Milk Supply</h3>
                <p>Fresh cow and buffalo milk delivered daily to your doorstep.</p>
            </div>
            <div class="service-item">
                <i class="fas fa-truck"></i>
                <h3>Milk Delivery</h3>
                <p>Reliable and timely delivery services for households and shops.</p>
            </div>
            <div class="service-item">
                <i class="fas fa-cheese"></i>
                <h3>Dairy Products</h3>
                <p>High-quality paneer, ghee, butter, curd and more from our farm.</p>
            </div>
        </div>
    </div>
</section>

<!-- Products Section -->
<section id="products">
    <div class="container">
        <h2>Our Products</h2>
        <div class="products-grid">
            <div class="product-item">
                <img src="https://i.pinimg.com/736x/b7/9d/4e/b79d4edbd482b4a390e771d13fd4869d.jpg" alt="Milk">
                <h4>Fresh Milk</h4>
            </div>
            <div class="product-item">
                <img src="https://i.pinimg.com/1200x/06/9d/e3/069de3677aae1469ea465457c3cb48ec.jpg" alt="Ghee">
                <h4>Ghee</h4>
            </div>
            <div class="product-item">
                <img src="https://i.pinimg.com/736x/ef/10/90/ef1090285e00e0960339555d9f860d3d.jpg" alt="Paneer">
                <h4>Paneer</h4>
            </div>
            <div class="product-item">
                <img src="https://i.pinimg.com/1200x/b9/48/9f/b9489f0d35d3c2f336dd688bb9a4a569.jpg" alt="Curd">
                <h4>Curd</h4>
            </div>
        </div>
    </div>
</section>

<!-- Gallery Section -->
<section id="gallery">
    <div class="container">
        <h2>Gallery</h2>
        <div class="gallery-grid">
            <img src="https://i.pinimg.com/1200x/63/f2/8c/63f28c4231bd462eb264000df8ace166.jpg" alt="Cow">
            <img src="https://i.pinimg.com/1200x/62/a1/e7/62a1e745e84eab9505fc965ab85386ab.jpg" alt="Cows in shed">
            <img src="https://i.pinimg.com/736x/1c/17/1f/1c171ff0f6c20cdf872165ff7864ea1e.jpg" alt="Buffalo milking">
            <img src="https://i.pinimg.com/1200x/cf/38/80/cf3880e2a22a178556c46bb09ff6352a.jpg" alt="Farm landscape">
        </div>
    </div>
</section>

<!-- Contact Section -->
<section id="contact">
    <div class="container">
        <h2>Contact Us</h2>
        <p>Phone: +91-8767444350 | Email: ajinkyabhandari112@gmail.com</p>
        <form id="contact-form">
            <input type="text" placeholder="Name" required>
            <input type="email" placeholder="Email" required>
            <textarea placeholder="Message" required></textarea>
            <button type="submit">Send Message</button>
        </form>
    </div>
</section>

<!-- Footer -->
<footer>
    <div class="container">
        <p>&copy; 2025 Ajinkya Dairy Farm. All rights reserved.</p>
        <div class="socials">
            <a href="#"><i class="fab fa-facebook-f"></i></a>
            <a href="#"><i class="fab fa-whatsapp"></i></a>
            <a href="#"><i class="fab fa-instagram"></i></a>
        </div>
    </div>
</footer>

<script src="script.js"></script>
</body>
</html>

document.querySelectorAll('nav a').forEach(link => {
    link.addEventListener('click', e => {
        e.preventDefault();
        document.querySelector(link.getAttribute('href')).scrollIntoView({ behavior: 'smooth' });
    });
});

document.getElementById('contact-form').addEventListener('submit', e => {
    e.preventDefault();
    alert('Thank you! Your message has been sent.');
});

* { margin: 0; padding: 0; box-sizing: border-box; font-family: Arial, sans-serif; }
body {
    font-family: 'Lato', sans-serif; /* keep your font */
    line-height: 1.6;
    background-color: #b7e3ea; /* CHANGE THIS COLOR */
}
.container { width: 90%; max-width: 1200px; margin: auto; }

header { background: #1087bd; color: #ffffff; padding: 20px 0; position: sticky; top: 0; z-index: 1000; }
header .logo { font-size: 24px; font-weight: bold; }
header nav ul { list-style: none; display: flex; gap: 20px; }
header nav ul li a { color: #fff; text-decoration: none; font-weight: bold; }

.hero { background: url('https://i.pinimg.com/1200x/b1/60/fd/b160fd1400433638e2e48fed6ab0b849.jpg') no-repeat center center/cover; color: #fff; padding: 100px 0; text-align: right; }
.hero h1 { font-size: 48px; margin-bottom: 20px; text-shadow: 2px 2px #000; }
.hero p { font-size: 20px; margin-bottom: 30px; text-shadow: 1px 1px #000; }
.btn { display: inline-block; padding: 10px 30px; background: #fff; color: #000000; text-decoration: none; border-radius: 5px; font-weight: bold; }

section { padding: 80px 0; text-align: center; }
.team-grid { display: flex; justify-content: center; gap: 30px; flex-wrap: wrap; margin-top: 40px; }
.team-member img { width: 150px; border-radius: 50%; }
.team-member h4 { margin-top: 10px; }
.team-member p { color: #555; }

.services-grid { display: flex; gap: 30px; justify-content: center; flex-wrap: wrap; margin-top: 40px; }
.service-item { background: #f4f4f4; padding: 30px; border-radius: 10px; width: 250px; transition: 0.3s; }
.service-item:hover { background: #000500; color: #fff; }
.service-item i { font-size: 40px; margin-bottom: 15px; }

.products-grid { display: flex; gap: 20px; justify-content: center; flex-wrap: wrap; margin-top: 40px; }
.product-item img { width: 300px; height: 200px; object-fit: cover; border-radius: 10px; }
.product-item h4 { margin-top: 10px; }

.gallery-grid { display: flex; gap: 20px; justify-content: center; flex-wrap: wrap; margin-top: 40px; }
.gallery-grid img { width: 300px; height: 200px; object-fit: cover; border-radius: 10px; }

#contact-form { display: flex; flex-direction: column; gap: 15px; max-width: 500px; margin: auto; }
#contact-form input, #contact-form textarea { padding: 10px; border-radius: 5px; border: 1px solid #ccc; width: 100%; }
#contact-form button { padding: 10px; border: none; border-radius: 5px; background: #000000; color: #fff; font-weight: bold; cursor: pointer; }

footer { background: #05719c; color: #fff; padding: 30px 0; text-align: center; }
footer .socials a { color: #fff; margin: 0 10px; text-decoration: none; font-size: 18px; }

@media (max-width: 768px) {
    header nav ul { flex-direction: column; gap: 10px; }
    .services-grid, .team-grid, .products-grid, .gallery-grid { flex-direction: column; align-items: center; }
    .hero h1 { font-size: 32px; }
}
/* Headings for the whole site */
h1, h2, h3 { font-family: 'Poppins', Showcard Gothic; }

/* Paragraphs / body text */
p { font-family: 'Lato', Bahnschrift Conde; }

/* Buttons */
button, .btn { font-family: 'Roboto', Showcard Gothic; }

/* About section */
#about p { font-family: 'Lato', Bahnschrift Conde; font-size: 18px; }

/* Services titles */
#services h3 { font-family: 'Poppins',Stencil; }

/* Products captions */
#products h4 { font-family: 'Roboto', sans-serif; }

/* Footer text */
footer p { font-family: 'Lato', sans-serif; }
/* Add border to all images */
img {
    border: 5px solid #000000; /* Dark green border */
    border-radius: 10px;        /* Rounded corners */
    padding: 3px;               /* Space between image and border */
}
