# TAP-STORE
Best renewed device is hear
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Renewed Phones Store</title>
  <style>
    body {
      font-family: 'Arial', sans-serif;
      margin: 0;
      padding: 0;
      background: #f4f4f9;
      color: #333;
    }

    header {
      background-color: #2c3e50;
      color: white;
      padding: 30px 10px;
      text-align: center;
      box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
    }

    header h1 {
      font-size: 2.5rem;
      margin: 0;
    }

    header p {
      font-size: 1.2rem;
    }

    .products {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
      gap: 30px;
      padding: 40px 20px;
      justify-items: center;
    }

    .product {
      background-color: #fff;
      padding: 20px;
      border-radius: 12px;
      box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
      transition: transform 0.3s ease, box-shadow 0.3s ease;
      text-align: center;
    }

    .product:hover {
      transform: translateY(-10px);
      box-shadow: 0 8px 20px rgba(0, 0, 0, 0.1);
    }

    .product img {
      width: 100%;
      height: 200px;
      object-fit: cover;
      border-radius: 8px;
    }

    .product h3 {
      margin-top: 15px;
      font-size: 1.6rem;
      color: #333;
    }

    .product p {
      margin: 8px 0;
      font-size: 1.1rem;
      color: #777;
    }

    .buy-btn {
      background-color: #27ae60;
      color: white;
      padding: 12px;
      border: none;
      border-radius: 6px;
      cursor: pointer;
      width: 100%;
      font-size: 1.1rem;
      margin-top: 15px;
      transition: background-color 0.3s ease;
    }

    .buy-btn:hover {
      background-color: #2ecc71;
    }

    .checkout {
      padding: 40px;
      text-align: center;
      background-color: #fff;
      box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
      border-radius: 12px;
      margin: 20px auto;
      width: 80%;
      max-width: 600px;
      display: none;
    }

    .checkout h2 {
      font-size: 2rem;
      margin-bottom: 20px;
    }

    .checkout p {
      font-size: 1.2rem;
      margin-bottom: 15px;
    }

    input[type="file"] {
      padding: 12px;
      margin-top: 10px;
      border-radius: 6px;
      border: 1px solid #ccc;
    }

    .footer {
      text-align: center;
      padding: 20px;
      background-color: #2c3e50;
      color: white;
      margin-top: 40px;
    }

    .footer p {
      margin: 0;
    }
  </style>
</head>

<body>
  <header>
    <h1>Renewed Phones Store</h1>
    <p>Best Quality, Affordable Prices</p>
  </header>

  <section class="products">
    <div class="product">
      <img src="https://via.placeholder.com/300x200" alt="iPhone XR">
      <h3>iPhone XR</h3>
      <p>Price: ₹18,999</p>
      <p>Condition: Like New</p>
      <button class="buy-btn" onclick="goToCheckout('iPhone XR', 18999)">Buy Now</button>
    </div>

    <div class="product">
      <img src="https://via.placeholder.com/300x200" alt="Samsung Galaxy S10">
      <h3>Samsung Galaxy S10</h3>
      <p>Price: ₹15,499</p>
      <p>Condition: Very Good</p>
      <button class="buy-btn" onclick="goToCheckout('Samsung Galaxy S10', 15499)">Buy Now</button>
    </div>

    <div class="product">
      <img src="https://via.placeholder.com/300x200" alt="iPhone 11">
      <h3>iPhone 11</h3>
      <p>Price: ₹25,999</p>
      <p>Condition: Like New</p>
      <button class="buy-btn" onclick="goToCheckout('iPhone 11', 25999)">Buy Now</button>
    </div>

    <!-- Add more products here in the same format -->
  </section>

  <div class="checkout" id="checkout">
    <h2>Checkout</h2>
    <p id="product-info"></p>
    <p>Please pay using Fampay UPI to: <strong>yourname@fam</strong></p>
    <p>After payment, upload your payment screenshot below:</p>
    <input type="file" accept="image/*">
  </div>

  <div class="footer">
    <p>&copy; 2025 Renewed Phones Store | All rights reserved.</p>
  </div>

  <script>
    function goToCheckout(product, price) {
      document.querySelector('.products').style.display = 'none';
      document.getElementById('checkout').style.display = 'block';
      document.getElementById('product-info').innerText = `You are buying: ${product} for ₹${price}`;
    }
  </script>
</body>
</html>
