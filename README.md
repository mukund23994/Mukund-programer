<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Indian Seller - Shop</title>

<style>
body {
    margin: 0;
    font-family: Arial, sans-serif;
    background: #f4f4f4;
}
header {
    background: #1a73e8;
    padding: 18px;
    color: white;
    font-size: 26px;
    text-align: center;
    font-weight: bold;
}
.container {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
}
.card {
    background: white;
    width: 320px;
    margin: 15px;
    border-radius: 12px;
    padding: 15px;
    text-align: center;
    box-shadow: 0px 4px 8px rgba(0,0,0,0.2);
}
.card img {
    width: 100%;
    border-radius: 10px;
}
button {
    background: #1a73e8;
    color: white;
    padding: 10px 20px;
    border: none;
    border-radius: 8px;
    cursor: pointer;
    margin-top: 10px;
    font-size: 16px;
}
button:hover {
    background: #0f5cc8;
}

/* Cart box */
#cartBox {
    background: #fff7d1;
    padding: 10px;
    margin: 10px;
    border: 2px solid #ffcc00;
    border-radius: 10px;
    display: none;
    width: 90%;
    max-width: 500px;
}
</style>

<script>
// Cart system
let cart = [];

function addToCart(item) {
    cart.push(item);
    document.getElementById("cartBox").style.display = "block";
    document.getElementById("cartList").innerHTML = cart.join("<br>");
}
</script>

</head>

<body>

<header>Indian Seller - Online Shopping</header>

<center>
<div id="cartBox">
    <h3>🛒 Your Cart</h3>
    <div id="cartList"></div>
</div>
</center>

<div class="container">

    <div class="card">
        <img src="https://i.imgur.com/Ap8W6sP.jpeg" alt="Tshirt">
        <h2>Stylish T-Shirt</h2>
        <p>₹299</p>
        <button onclick="addToCart('Stylish T-Shirt - ₹299')">Add to Cart</button>
    </div>

    <div class="card">
        <img src="https://i.imgur.com/fP3kH2G.jpeg" alt="Jeans">
        <h2>Blue Denim Jeans</h2>
        <p>₹799</p>
        <button onclick="addToCart('Blue Jeans - ₹799')">Add to Cart</button>
    </div>

    <div class="card">
        <img src="https://i.imgur.com/sq3tYED.jpeg" alt="Hoodie">
        <h2>Winter Hoodie</h2>
        <p>₹999</p>
        <button onclick="addToCart('Hoodie - ₹999')">Add to Cart</button>
    </div>

</div>

</body>
</html>
