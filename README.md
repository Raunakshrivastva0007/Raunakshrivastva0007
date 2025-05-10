<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Aman Service Center</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background-color: #f9f9f9;
    }

    header {
      background-color: #004080;
      color: white;
      padding: 20px;
      text-align: center;
    }

    .about {
      padding: 30px;
      background-color: #ffffff;
      text-align: center;
    }

    .about h2 {
      color: #004080;
    }

    .slider {
      width: 100%;
      overflow: hidden;
      margin: 0 auto;
    }

    .slider img {
      width: 100%;
      height: auto;
      display: block;
    }

    .service {
      padding: 20px;
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 20px;
      background-color: #eef4f7;
    }

    .service-box {
      background: white;
      border-radius: 10px;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
      padding: 15px;
      width: 250px;
      text-align: center;
    }

    .service-box img {
      max-width: 100%;
      height: 150px;
      border-radius: 10px;
    }

    .buttons {
      text-align: center;
      margin: 30px 0;
    }

    .buttons button, .buttons a {
      display: inline-block;
      margin: 10px;
      padding: 12px 25px;
      background-color: #28a745;
      color: white;
      text-decoration: none;
      border-radius: 5px;
      font-weight: bold;
      cursor: pointer;
      border: none;
    }

    .form-container {
      perspective: 1000px;
      text-align: center;
    }

    .form-card {
      width: 100%;
      max-width: 500px;
      margin: 0 auto;
      transform-style: preserve-3d;
      transition: transform 0.8s;
    }

    .form-card.flipped {
      transform: rotateY(180deg);
    }

    .form-front, .form-back {
      backface-visibility: hidden;
      position: absolute;
      width: 100%;
      padding: 20px;
      box-sizing: border-box;
      border-radius: 10px;
      box-shadow: 0 0 10px rgba(0,0,0,0.2);
      background: #fff;
    }

    .form-back {
      transform: rotateY(180deg);
    }

    form input, form textarea {
      width: 100%;
      padding: 10px;
      margin: 10px 0;
      border: 1px solid #ccc;
      border-radius: 5px;
      box-sizing: border-box;
    }

    footer {
      background-color: #333;
      color: white;
      text-align: center;
      padding: 20px;
    }
  </style>
  <script>
    function flipForm() {
      document.querySelector('.form-card').classList.toggle('flipped');
    }
  </script>
</head>
<body>

  <header>
    <h1>Aman Service Center</h1>
    <p>AC, Refrigerator, RO, Cooler & All Appliances Repair and Sales - Mangolpuri, Delhi</p>
  </header>

  <div class="slider">
    <img src="https://i.imgur.com/RWIVpG0.jpg" alt="Technician at Work">
    <img src="https://i.imgur.com/sZkFf8N.jpg" alt="Home Appliance Service">
    <img src="https://i.imgur.com/4YUw6me.jpg" alt="Repair Expert">
  </div>

  <div class="about">
    <h2>About Us</h2>
    <p>Welcome to Aman Service Center! We are based in Mangolpuri, New Delhi 110083 and offer expert services in repair and sales of Air Conditioners (AC), Refrigerators, RO Water Purifiers, Coolers, and all other home appliances. With trained technicians and reliable support, we provide efficient, affordable, and trustworthy solutions for your household electronic needs. Whether you need installation, maintenance, or urgent repairs, our team is available to assist you at your doorstep.</p>
  </div>

  <div class="service">
    <div class="service-box">
      <img src="https://i.imgur.com/8UAYqKZ.jpg" alt="AC Service">
      <h3>AC Repair & Installation</h3>
    </div>
    <div class="service-box">
      <img src="https://i.imgur.com/DQaGvDT.jpg" alt="Refrigerator">
      <h3>Refrigerator Repair</h3>
    </div>
    <div class="service-box">
      <img src="https://i.imgur.com/Yw7mEv2.jpg" alt="RO System">
      <h3>RO System Service</h3>
    </div>
    <div class="service-box">
      <img src="https://i.imgur.com/hCVzQ7z.jpg" alt="Cooler Repair">
      <h3>Cooler Maintenance</h3>
    </div>
    <div class="service-box">
      <img src="https://i.imgur.com/mXuwJev.jpg" alt="All Appliance">
      <h3>All Home Appliances</h3>
    </div>
  </div>

  <div class="buttons">
    <button onclick="flipForm()">🔧 Book a Service (Form)</button>
    <a href="https://wa.me/919811506810?text=Hi%20Aman%20Service%20Center%2C%20I%20need%20help%20with%20an%20appliance">💬 Contact on WhatsApp</a>
    <a href="tel:9811506810">📞 Call: 9811506810</a>
  </div>

  <div class="form-container">
    <div class="form-card">
      <div class="form-front">
        <p>Click the button above to flip and fill the service form.</p>
      </div>
      <div class="form-back">
        <form action="mailto:your-email@example.com" method="post" enctype="text/plain">
          <input type="text" name="name" placeholder="Your Name" required>
          <input type="text" name="phone" placeholder="Phone Number" required>
          <input type="text" name="address" placeholder="Address" required>
          <input type="text" name="product" placeholder="Product (AC, Fridge, etc.)" required>
          <textarea name="problem" rows="4" placeholder="Describe the issue..." required></textarea>
          <input type="submit" value="Submit">
        </form>
      </div>
    </div>
  </div>

  <footer>
    <p>&copy; 2025 Aman Service Center | Mangolpuri, Delhi</p>
  </footer>

</body>
</html>
