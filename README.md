# Al-Masar-Travel-and-Tourism-Co
Al Masar Travels - Tours, pricing, and booking site
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Al Masar Travels & Tourism</title>
  <style>
    body { font-family: Arial, sans-serif; margin: 0; padding: 0; background: #f4f4f4; }
    
    /* Header */
    header { 
      background: url('https://via.placeholder.com/1200x400?text=Al+Masar+Travels') center/cover no-repeat; 
      color: white; text-align: center; padding: 100px 20px; 
    }
    header h1 { margin: 0; font-size: 2.5em; text-shadow: 2px 2px 6px rgba(0,0,0,0.5); }
    header p { font-size: 1.2em; text-shadow: 1px 1px 4px rgba(0,0,0,0.5); }
    header a { color: #1abc9c; text-decoration: none; }

    /* Section styles */
    section { max-width: 1000px; margin: 30px auto; background: white; padding: 20px; border-radius: 8px; box-shadow: 0 0 10px rgba(0,0,0,0.1); }
    h2 { color: #2c3e50; margin-top: 0; }
    p, li { line-height: 1.6; }
    .contact a { color: #1abc9c; text-decoration: none; }

    /* Contact form */
    form { display: flex; flex-direction: column; }
    input, textarea { padding: 10px; margin-bottom: 15px; border: 1px solid #ccc; border-radius: 4px; font-size: 1em; }
    button { padding: 12px; background: #1abc9c; color: white; border: none; border-radius: 4px; cursor: pointer; font-size: 1em; }
    button:hover { background: #16a085; }

    /* Tour Gallery Grid */
    .tours-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 20px;
    }
    .tour-card {
      position: relative;
      border-radius: 10px;
      overflow: hidden;
      box-shadow: 0 5px 15px rgba(0,0,0,0.2);
      transition: transform 0.3s, box-shadow 0.3s;
      background: #fff;
    }
    .tour-card img {
      width: 100%;
      height: 220px;
      object-fit: cover;
      display: block;
    }
    .tour-card:hover {
      transform: translateY(-5px);
      box-shadow: 0 10px 25px rgba(0,0,0,0.3);
    }
    .tour-info {
      padding: 15px;
      text-align: center;
    }
    .tour-info h3 {
      margin: 10px 0 5px 0;
      font-size: 1.2em;
      color: #2c3e50;
    }
    .tour-info p {
      font-size: 0.95em;
      color: #555;
      margin: 5px 0;
    }
    .price {
      font-weight: bold;
      color: #1abc9c;
      margin: 10px 0;
      font-size: 1.1em;
    }
    .book-btn {
      display: inline-block;
      padding: 10px 20px;
      background: #1abc9c;
      color: white;
      text-decoration: none;
      border-radius: 5px;
      transition: background 0.3s;
    }
    .book-btn:hover { background: #16a085; }

    /* Responsive */
    @media(max-width: 768px){ .tour-card img { height: 180px; } }
    @media(max-width: 500px){ header { padding: 60px 20px; } }

    footer { text-align: center; padding: 20px; font-size: 0.9em; color: #555; }
  </style>
</head>
<body>

<header>
  <h1>Al Masar Travels & Tourism</h1>
  <p>Follow us on Instagram: <a href="https://www.instagram.com/almasartravels" target="_blank">@almasartravels</a></p>
</header>

<section class="contact">
  <h2>Contact Information</h2>
  <p>Email: <a href="mailto:almasartravels@gmail.com">almasartravels@gmail.com</a></p>
  <p>Phone: +92 313 8855110 / (021) 32237271</p>
  <p>Address: C‑432, 1st Floor, Allama Iqbal Rd, P.E.C.H.S Block 2, Karachi, Pakistan</p>
  <p>Website: <a href="https://www.almasartravels.com.pk" target="_blank">www.almasartravels.com.pk</a></p>
</section>

<section>
  <h2>Our Tours</h2>
  <div class="tours-grid">
    <!-- Tour 1 -->
    <div class="tour-card">
      <img src="https://via.placeholder.com/400x300?text=Beach+Adventure" alt="Beach Adventure">
      <div class="tour-info">
        <h3>Beach Adventure</h3>
        <p>Explore Karachi's stunning beaches with a guided adventure.</p>
        <p class="price">PKR 25,000</p>
        <a href="#contact-form" class="book-btn">Book Now</a>
      </div>
    </div>
    <!-- Tour 2 -->
    <div class="tour-card">
      <img src="https://via.placeholder.com/400x300?text=City+Heritage+Tour" alt="City Heritage Tour">
      <div class="tour-info">
        <h3>City Heritage Tour</h3>
        <p>Discover Karachi's historical landmarks and vibrant streets.</p>
        <p class="price">PKR 18,000</p>
        <a href="#contact-form" class="book-btn">Book Now</a>
      </div>
    </div>
    <!-- Tour 3 -->
    <div class="tour-card">
      <img src="https://via.placeholder.com/400x300?text=Desert+Safari" alt="Desert Safari">
      <div class="tour-info">
        <h3>Desert Safari</h3>
        <p>Experience thrilling rides across the Sindh desert dunes.</p>
        <p class="price">PKR 35,000</p>
        <a href="#contact-form" class="book-btn">Book Now</a>
      </div>
    </div>
  </div>
</section>

<section id="contact-form">
  <h2>Book Your Tour / Send Inquiry</h2>
  <form action="mailto:almasartravels@gmail.com" method="post" enctype="text/plain" target="_blank">
    <label for="name">Name</label>
    <input type="text" id="name" name="name" placeholder="Your Name" required>

    <label for="email">Email</label>
    <input type="email" id="email" name="email" placeholder="Your Email" required>

    <label for="phone">Phone</label>
    <input type="text" id="phone" name="phone" placeholder="Phone Number" required>

    <label for="message">Message</label>
    <textarea id="message" name="message" placeholder="Your Message or Tour Inquiry" rows="5" required></textarea>

    <button type="submit">Send Inquiry</button>
  </form>
</section>

<footer>
  &copy; 2026 Al Masar Travels & Tourism. All rights reserved.
</footer>

</body>
</html>
