<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Ganpati Mobile House</title>
  <style>
    * { box-sizing: border-box; }
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: #f0f0f0;
    }
    header {
      background: #2e3192;
      color: white;
      padding: 20px;
      position: relative;
    }
    .ceo {
      position: absolute;
      top: 10px;
      left: 10px;
      font-size: 14px;
    }
    .title {
      text-align: center;
      font-size: 28px;
      font-weight: bold;
    }
    .tagline {
      text-align: center;
      font-size: 16px;
      margin-top: 5px;
    }
    nav {
      background: #444;
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
    }
    nav a {
      padding: 10px 15px;
      color: white;
      text-decoration: none;
      background: #007bff;
      border-radius: 5px;
      margin: 5px;
    }
    #search-bar {
      width: 90%;
      margin: 10px auto;
      padding: 10px;
      font-size: 16px;
      display: block;
      border-radius: 5px;
    }
    section {
      background: white;
      margin: 10px;
      padding: 20px;
      border-radius: 10px;
    }
    h2 { color: #2e3192; }
    img {
      max-width: 100%;
      height: auto;
      margin-bottom: 10px;
      border-radius: 10px;
    }
    .product {
      margin-bottom: 20px;
    }
    .footer {
      background: #2e3192;
      color: white;
      text-align: center;
      padding: 15px;
      margin-top: 30px;
    }
    .back-to-top {
      display: block;
      margin: 20px auto;
      text-align: center;
      color: #fff;
      background: #28a745;
      padding: 10px;
      border-radius: 5px;
      width: 150px;
      text-decoration: none;
    }
  </style>
  <script>
    function filterProducts() {
      const query = document.getElementById('search-bar').value.toLowerCase();
      const products = document.querySelectorAll('.product');
      products.forEach(p => {
        const text = p.textContent.toLowerCase();
        p.style.display = text.includes(query) ? '' : 'none';
      });
    }
  </script>
</head>
<body>

  <header>
    <div class="ceo">CEO: Amit Sharma</div>
    <div class="title">Ganpati Mobile House</div>
    <div class="tagline">Everything Digital, All in One Place.</div>
  </header>

  <nav>
    <a href="#mobiles">Mobiles</a>
    <a href="#accessories">Accessories</a>
    <a href="#laptops">Laptops</a>
    <a href="#electronics">Electronics</a>
    <a href="#computers">Computers</a>
    <a href="#contact">Contact</a>
  </nav>

  <input type="text" id="search-bar" onkeyup="filterProducts()" placeholder="Search products...">

  <section id="mobiles">
    <h2>Mobiles</h2>
    <div class="product">
      <h3>Oppo Reno11 - ₹27,999</h3>
      <img src="https://www.oppo.com/content/dam/oppo/common/mkt/v2-2/reno11/navigation/reno11-navigation-green.png" alt="Oppo Reno11">
    </div>
    <div class="product">
      <h3>Realme Narzo 70 Pro - ₹18,999</h3>
      <img src="https://fdn2.gsmarena.com/vv/pics/realme/realme-narzo-70-pro-5g-1.jpg" alt="Realme Narzo 70 Pro">
    </div>
    <div class="product">
      <h3>POCO X5 Pro - ₹20,999</h3>
      <img src="https://fdn2.gsmarena.com/vv/pics/xiaomi/xiaomi-poco-x5-pro-1.jpg" alt="POCO X5 Pro">
    </div>
    <div class="product">
      <h3>Tecno Spark 10 - ₹8,999</h3>
      <img src="https://fdn2.gsmarena.com/vv/pics/tecno/tecno-spark-10-1.jpg" alt="Tecno Spark 10">
    </div>
    <div class="product">
      <h3>Vivo Y200 5G - ₹21,999</h3>
      <img src="https://fdn2.gsmarena.com/vv/pics/vivo/vivo-y200-5g-1.jpg" alt="Vivo Y200">
    </div>
  </section>

  <section id="accessories">
    <h2>Accessories</h2>
    <div class="product">Realme Buds Wireless - ₹1,299</div>
    <div class="product">OPPO Charger - ₹899</div>
    <div class="product">Vivo Earphones - ₹499</div>
    <div class="product">POCO Power Bank - ₹1,199</div>
  </section>

  <section id="laptops">
    <h2>Laptops</h2>
    <div class="product">Dell Inspiron 15 (i5 12th Gen) - ₹49,999</div>
    <div class="product">HP Pavilion x360 (i3 11th Gen, Touch) - ₹44,990</div>
    <div class="product">Lenovo IdeaPad Slim 3 (Ryzen 5, 16GB) - ₹42,990</div>
    <div class="product">Asus VivoBook 14 (i5, SSD) - ₹38,999</div>
  </section>

  <section id="electronics">
    <h2>Electronics</h2>
    <h3>AC</h3>
    <div class="product">Blue Star 1 Ton 5 Star - ₹37,490</div>
    <h3>Washing Machines</h3>
    <div class="product">LG 8 Kg Front Load - ₹34,990</div>
    <h3>Refrigerator</h3>
    <div class="product">Samsung 253L Double Door - ₹23,990</div>
    <h3>Cooler</h3>
    <div class="product">Symphony Ice Cube 27 - ₹5,490</div>
    <h3>Microwave</h3>
    <div class="product">IFB 20 L Convection - ₹9,490</div>
    <h3>TV</h3>
    <div class="product">TCL 40" Smart TV - ₹15,990</div>
  </section>

  <section id="computers">
    <h2>Computers</h2>
    <div class="product">Assembled CPU (i5, 8GB RAM, 512GB SSD) - ₹23,000</div>
    <div class="product">Logitech Keyboard & Mouse Combo - ₹999</div>
    <div class="product">Intel Core i7 Processor - ₹21,000</div>
    <div class="product">Gigabyte B660 Motherboard - ₹9,500</div>
  </section>

  <section id="contact">
    <h2>Contact Us</h2>
    <p>Location: Near Main Market, Lunkaransar, Bikaner District, Rajasthan</p>
    <p>Phone: +91-9876543210</p>
    <p>Hours: 10 AM – 9 PM (All Days)</p>
  </section>

  <a href="#top" class="back-to-top">Back to Top</a>

  <div class="footer">
    © 2025 Ganpati Mobile House | CEO: Amit Sharma | Built with Passion
  </div>

</body>
</html>
