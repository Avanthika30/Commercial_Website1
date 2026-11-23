# Ex02 Commercial Website
## Date: 23.11.2026
## Reg.no: 212224040039
## AIM
To create a commercial website using CSS Flexbox.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for Homepage, Products / Services, About Us, Contact Details and User Account.

### STEP 5
Include social media links at the footer with copyright information.

### STEP 6
Define global styles for fonts, colors, and layout.

### STEP 7
Style the header, navigation bar, and sections.

### STEP 8
Use Flexbox for layout design.

### STEP 9
Add hover effects and transitions for interactivity.

### STEP 10
Add Images and Media.

### STEP 11
Use optimized images for a professional look.

### STEP 12
Open the HTML file in a browser to check layout and functionality.

### STEP 13
Fix styling issues and refine content placement.

### STEP 14
Deploy the website.

### STEP 15
Upload to GitHub Pages for free hosting.

## PROGRAM

### Index.html:
```

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Brewly - Fresh Coffee & Bakes</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>

<!-- NAVBAR -->
<header class="navbar">
  <a class="logo" href="#top">Brew<span>ly</span></a>

  <ul class="nav-links">
    <li><a href="#top">Home</a></li>
    <li><a href="#features">Why Us</a></li>
    <li><a href="#products">Products</a></li>
    <li><a href="#contact">Contact</a></li>
  </ul>

  <a class="btn cart-nav" href="#cart">
    🛒 Cart <span id="cart-count">0</span>
  </a>
</header>

<main id="top">

  <!-- HERO -->
  <section class="hero">
    <div class="hero-text">
      <p class="tag">Freshly roasted daily</p>
      <h1>Great coffee,<br>delivered to your door.</h1>
      <p class="lead">
        Small-batch beans, warm bakes and handcrafted blends.
        Order online and enjoy the cafe experience at home.
      </p>
      <div class="hero-buttons">
        <a class="btn" href="#products">Order Now</a>
        <a class="btn outline" href="#features">Learn More</a>
      </div>
    </div>

    <div class="hero-photo">
      <img src="download (1).jpg" alt="Cozy Brewly cafe interior">
    </div>
  </section>

  <!-- FEATURES -->
  <section class="features" id="features">
    <div class="feature">
      <span class="icon">🚚</span>
      <h3>Free Delivery</h3>
      <p>On every order above Rs. 499.</p>
    </div>
    <div class="feature">
      <span class="icon">🌿</span>
      <h3>100% Fresh</h3>
      <p>Roasted and packed within 48 hours.</p>
    </div>
    <div class="feature">
      <span class="icon">💳</span>
      <h3>Secure Payment</h3>
      <p>UPI, cards and cash on delivery.</p>
    </div>
  </section>

  <!-- PRODUCTS -->
  <section class="section" id="products">
    <h2>Our Best Sellers</h2>
    <p class="sub">Pick your favourites and add them to the cart.</p>

    <div class="products">

      <article class="product">
        <div class="pic">
          <img src="Filter Coffee.jpg" alt="Classic filter coffee">
        </div>
        <span class="category">Coffee</span>
        <h3>Classic Filter Coffee</h3>
        <p>Rich South Indian decoction blend, 250 g.</p>
        <div class="buy">
          <b>Rs. 299</b>
          <button class="btn small add-btn"
            data-id="1">Add to Cart</button>
        </div>
      </article>

      <article class="product">
        <div class="pic">
          <img src="15 Easy Iced Coffee Recipes _ Homemade Drinks.jpg"
            alt="Iced Cold Brew">
        </div>
        <span class="category">Beverage</span>
        <h3>Iced Cold Brew</h3>
        <p>Smooth, slow-steeped for 18 hours, 500 ml.</p>
        <div class="buy">
          <b>Rs. 199</b>
          <button class="btn small add-btn"
            data-id="2">Add to Cart</button>
        </div>
      </article>

      <article class="product">
        <div class="pic">
          <img src="download (3).jpg" alt="Butter Croissant">
        </div>
        <span class="category">Bakery</span>
        <h3>Butter Croissant</h3>
        <p>Flaky and baked fresh every morning.</p>
        <div class="buy">
          <b>Rs. 89</b>
          <button class="btn small add-btn"
            data-id="3">Add to Cart</button>
        </div>
      </article>

      <article class="product">
        <div class="pic">
          <img src="download (4).jpg" alt="Choco Chip Cookies">
        </div>
        <span class="category">Bakery</span>
        <h3>Choco Chip Cookies</h3>
        <p>Pack of 6 with dark chocolate chunks.</p>
        <div class="buy">
          <b>Rs. 149</b>
          <button class="btn small add-btn"
            data-id="4">Add to Cart</button>
        </div>
      </article>

    </div>
  </section>

  <!-- SHOPPING CART -->
  <section class="section cart-section" id="cart">
    <h2>Your Shopping Cart 🛒</h2>
    <p class="sub">Review your selected coffee and treats.</p>

    <div class="cart-layout">

      <div class="cart-items">
        <div id="cart-items">
          <div class="empty-cart">
            <span>🛍️</span>
            <h3>Your cart is empty!</h3>
            <p>Looks like you haven't added anything yet.</p>
            <a href="#products" class="btn">Explore Products</a>
          </div>
        </div>
      </div>

      <!-- BILL SUMMARY -->
      <div class="bill-card">
        <h3>Order Summary</h3>

        <div class="bill-line">
          <span>Subtotal</span>
          <span id="subtotal">Rs. 0.00</span>
        </div>

        <div class="bill-line">
          <span>Delivery Fee</span>
          <span id="delivery">Rs. 40.00</span>
        </div>

        <div class="bill-line">
          <span>Discount</span>
          <span id="discount">- Rs. 0.00</span>
        </div>

        <div class="bill-line">
          <span>GST (5%)</span>
          <span id="gst">Rs. 0.00</span>
        </div>

        <hr>

        <div class="bill-line total">
          <span>Total Amount</span>
          <span id="grand-total">Rs. 0.00</span>
        </div>

        <p class="offer-note">
          🎉 Free delivery on orders above Rs. 499!
        </p>

        <button class="btn checkout-btn" id="checkout-btn" disabled>
          Proceed to Checkout →
        </button>
      </div>

    </div>
  </section>

  <!-- CHECKOUT -->
  <section class="section checkout-section" id="checkout">
    <h2>Checkout</h2>
    <p class="sub">Just a few details before your Brewly order arrives!</p>

    <div class="checkout-layout">

      <form id="checkout-form" class="checkout-form">

        <h3>Customer Information</h3>

        <label for="customer-name">Full Name</label>
        <input type="text" id="customer-name"
          placeholder="Enter your full name" required>

        <label for="phone">Mobile Number</label>
        <input type="tel" id="phone"
          placeholder="10-digit mobile number"
          pattern="[6-9][0-9]{9}" maxlength="10" required>

        <label for="email">Email Address</label>
        <input type="email" id="email"
          placeholder="example@email.com" required>

        <label for="address">Delivery Address</label>
        <textarea id="address" rows="3"
          placeholder="House no., Street, Area, City, PIN code"
          required></textarea>

        <h3>Payment Method</h3>

        <label class="payment-option">
          <input type="radio" name="payment" value="UPI" required>
          UPI Payment
        </label>

        <label class="payment-option">
          <input type="radio" name="payment" value="Card">
          Credit / Debit Card
        </label>

        <label class="payment-option">
          <input type="radio" name="payment" value="COD">
          Cash on Delivery
        </label>

        <button type="submit" class="btn place-order-btn">
          Place Order
        </button>

      </form>

      <div class="checkout-info">
        <h3>Why shop with Brewly?</h3>
        <p>☕ Freshly prepared products</p>
        <p>📦 Carefully packed orders</p>
        <p>🚚 Reliable doorstep delivery</p>
        <p>💳 Multiple payment options</p>
        <hr>
        <h3>Estimated Delivery</h3>
        <p>Within 30–45 minutes after order confirmation.</p>
      </div>

    </div>
  </section>

  <!-- ORDER SUCCESS -->
  <section class="section success-section" id="success" hidden>
    <div class="success-card">
      <div class="success-icon">✓</div>
      <h2>Order Placed Successfully!</h2>
      <p>Thank you for choosing Brewly. Your order is being prepared.</p>

      <div class="order-details">
        <p>Order ID: <b id="order-id"></b></p>
        <p>Customer: <b id="order-customer"></b></p>
        <p>Payment: <b id="order-payment"></b></p>
        <p>Total Paid: <b id="order-total"></b></p>
      </div>

      <button class="btn" id="continue-shopping">
        Continue Shopping
      </button>
    </div>
  </section>

  <!-- CTA -->
  <section class="cta">
    <h2>Get 10% off your first order</h2>
    <p>Fresh coffee tastes even better with a little discount!</p>
    <a class="btn" href="#products">Shop Now</a>
  </section>

</main>

<!-- FOOTER -->
<footer id="contact">
  <div class="footer-top">
    <div class="footer-col">
      <h4>Brewly</h4>
      <p>Fresh coffee and bakes, made with care.</p>
    </div>

    <div class="footer-col">
      <h4>Quick Links</h4>
      <a href="#top">Home</a>
      <a href="#products">Products</a>
      <a href="#features">Why Us</a>
      <a href="#cart">Shopping Cart</a>
    </div>

    <div class="footer-col">
      <h4>Contact</h4>
      <p>Chennai, Tamil Nadu</p>
      <p>hello@brewly.com</p>
      <p>+91 98765 43210</p>
    </div>
  </div>

  <div class="footer-bottom">
    <p>Name: <b>Avanthika Baskaran</b></p>
    <p>Register No: <b>212224040039</b></p>
    <p>Saveetha Engineering College</p>
  </div>
</footer>

<script>
let cart = [];

const products = [
  {id:1, name:"Classic Filter Coffee", price:299, image:"Filter Coffee.jpg"},
  {id:2, name:"Iced Cold Brew", price:199, image:"15 Easy Iced Coffee Recipes _ Homemade Drinks.jpg"},
  {id:3, name:"Butter Croissant", price:89, image:"download (3).jpg"},
  {id:4, name:"Choco Chip Cookies", price:149, image:"download (4).jpg"}
];

const money = n => "Rs. " + n.toFixed(2);

document.querySelectorAll(".add-btn").forEach(button => {
  button.addEventListener("click", () => {
    const id = Number(button.dataset.id);
    const item = cart.find(p => p.id === id);

    if (item) item.quantity++;
    else cart.push({id, quantity:1});

    updateCart();

    button.textContent = "Added ✓";
    setTimeout(() => button.textContent = "Add to Cart", 1000);
  });
});

function changeQuantity(id, amount) {
  const item = cart.find(p => p.id === id);
  if (!item) return;

  item.quantity += amount;

  if (item.quantity <= 0) removeProduct(id);
  else updateCart();
}

function removeProduct(id) {
  cart = cart.filter(p => p.id !== id);
  updateCart();
}

function updateCart() {
  const container = document.getElementById("cart-items");
  const count = document.getElementById("cart-count");

  let subtotal = 0;
  let quantity = 0;

  if (cart.length === 0) {
    container.innerHTML = `
      <div class="empty-cart">
        <span>🛍️</span>
        <h3>Your cart is empty!</h3>
        <p>Looks like you haven't added anything yet.</p>
        <a href="#products" class="btn">Explore Products</a>
      </div>`;
  } else {
    container.innerHTML = cart.map(item => {
      const p = products.find(x => x.id === item.id);
      const total = p.price * item.quantity;

      subtotal += total;
      quantity += item.quantity;

      return `
        <div class="cart-item">
          <img src="${p.image}" alt="${p.name}">
          <div class="cart-product-info">
            <h3>${p.name}</h3>
            <p>Freshly prepared by Brewly</p>
            <div class="cart-price">${money(p.price)}</div>
            <div class="quantity">
              <button type="button" onclick="changeQuantity(${p.id},-1)">−</button>
              <span>${item.quantity}</span>
              <button type="button" onclick="changeQuantity(${p.id},1)">+</button>
            </div>
            <button type="button" class="remove-btn" onclick="removeProduct(${p.id})">Remove</button>
          </div>
          <strong>${money(total)}</strong>
        </div>`;
    }).join("");
  }

  const delivery = subtotal === 0 || subtotal >= 499 ? 0 : 40;
  const discount = subtotal * 0.10;
  const gst = (subtotal - discount) * 0.05;
  const grandTotal = subtotal - discount + gst + delivery;

  count.textContent = quantity;
  document.getElementById("subtotal").textContent = money(subtotal);
  document.getElementById("delivery").textContent =
    delivery === 0 && subtotal > 0 ? "FREE" : money(delivery);
  document.getElementById("discount").textContent = "- " + money(discount);
  document.getElementById("gst").textContent = money(gst);
  document.getElementById("grand-total").textContent = money(grandTotal);

  document.getElementById("checkout-btn").disabled = cart.length === 0;

  return {subtotal, delivery, discount, gst, grandTotal};
}

document.getElementById("checkout-btn").addEventListener("click", () => {
  if (cart.length > 0) {
    document.getElementById("checkout").scrollIntoView({behavior:"smooth"});
  }
});

document.getElementById("checkout-form").addEventListener("submit", function(e) {
  e.preventDefault();

  if (cart.length === 0) {
    alert("Your cart is empty!");
    return;
  }

  const name = document.getElementById("customer-name").value.trim();
  const phone = document.getElementById("phone").value.trim();
  const payment = document.querySelector('input[name="payment"]:checked');

  if (!/^[6-9][0-9]{9}$/.test(phone)) {
    alert("Enter a valid 10-digit mobile number.");
    return;
  }

  if (!payment) {
    alert("Please select a payment method.");
    return;
  }

  const bill = updateCart();
  const orderId = "BRW" + Date.now().toString().slice(-8);

  document.getElementById("order-id").textContent = orderId;
  document.getElementById("order-customer").textContent = name;
  document.getElementById("order-payment").textContent =
    payment.value === "COD" ? "Cash on Delivery" : payment.value;
  document.getElementById("order-total").textContent = money(bill.grandTotal);

  document.getElementById("checkout").hidden = true;
  document.getElementById("cart").hidden = true;
  document.getElementById("products").hidden = true;
  document.getElementById("success").hidden = false;

  cart = [];
  updateCart();
  this.reset();

  document.getElementById("success").scrollIntoView({behavior:"smooth"});
});

document.getElementById("continue-shopping").addEventListener("click", () => {
  document.getElementById("success").hidden = true;
  document.getElementById("products").hidden = false;
  document.getElementById("cart").hidden = false;
  document.getElementById("checkout").hidden = false;

  document.getElementById("products").scrollIntoView({behavior:"smooth"});
});

updateCart();
</script>
</body>
</html>

```

### Style.css:
```

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

html {
  scroll-behavior: smooth;
}

body {
  font-family: 'Segoe UI', Arial, sans-serif;
  background: #fffaf5;
  color: #38251d;
  line-height: 1.6;
}

a {
  text-decoration: none;
  color: inherit;
}

button, input, textarea {
  font: inherit;
}

button {
  cursor: pointer;
}

/* NAVBAR */
.navbar {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 18px 8%;
  background: #fff;
  position: sticky;
  top: 0;
  z-index: 100;
  box-shadow: 0 2px 12px #0000000c;
}

.logo {
  font-size: 30px;
  font-weight: 800;
  color: #553321;
}

.logo span {
  color: #bd8050;
}

.nav-links {
  display: flex;
  list-style: none;
  gap: 30px;
}

.nav-links a:hover {
  color: #bd8050;
}

.btn {
  display: inline-block;
  background: #70462e;
  color: white;
  padding: 12px 23px;
  border: none;
  border-radius: 6px;
  font-weight: 600;
  transition: 0.3s;
  text-align: center;
}

.btn:hover {
  background: #a36b45;
  transform: translateY(-2px);
}

.cart-nav {
  display: flex;
  align-items: center;
  gap: 9px;
}

#cart-count {
  background: #fff;
  color: #70462e;
  border-radius: 50%;
  width: 23px;
  height: 23px;
  display: inline-flex;
  align-items: center;
  justify-content: center;
  font-size: 12px;
}

/* HERO */
.hero {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 75px 8%;
  gap: 50px;
}

.hero-text {
  flex: 1;
}

.tag {
  color: #a36b45;
  text-transform: uppercase;
  font-weight: 700;
  letter-spacing: 2px;
  font-size: 13px;
}

.hero h1 {
  font-size: clamp(36px, 5vw, 57px);
  line-height: 1.15;
  margin: 15px 0;
  color: #493024;
}

.lead {
  color: #76645a;
  max-width: 500px;
  margin-bottom: 25px;
}

.hero-buttons {
  display: flex;
  gap: 12px;
}

.outline {
  background: transparent;
  color: #70462e;
  border: 1px solid #70462e;
}

.outline:hover {
  color: white;
}

.hero-photo {
  flex: 1;
}

.hero-photo img {
  width: 100%;
  height: 390px;
  object-fit: cover;
  border-radius: 14px;
}

/* FEATURES */
.features {
  background: #f3e9df;
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  padding: 38px 8%;
  text-align: center;
  gap: 30px;
}

.icon {
  font-size: 32px;
}

.feature h3 {
  margin: 8px 0;
}

.feature p {
  color: #76645a;
  font-size: 14px;
}

/* GENERAL SECTIONS */
.section {
  padding: 65px 8%;
}

.section h2 {
  font-size: 32px;
  text-align: center;
  color: #493024;
}

.sub {
  text-align: center;
  color: #88776d;
  margin: 8px 0 35px;
}

/* PRODUCTS */
.products {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 25px;
}

.product {
  background: white;
  border-radius: 12px;
  padding: 15px;
  box-shadow: 0 4px 18px #0000000b;
  transition: 0.3s;
}

.product:hover {
  transform: translateY(-5px);
  box-shadow: 0 8px 25px #00000015;
}

.pic {
  overflow: hidden;
  border-radius: 9px;
  margin-bottom: 12px;
}

.pic img {
  width: 100%;
  height: 190px;
  object-fit: cover;
  display: block;
}

.category {
  display: inline-block;
  background: #f5e9dd;
  color: #986b4c;
  font-size: 11px;
  font-weight: 700;
  padding: 3px 10px;
  border-radius: 20px;
}

.product h3 {
  margin: 9px 0 5px;
}

.product p {
  color: #82736a;
  font-size: 13px;
  min-height: 42px;
}

.buy {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 8px;
  margin-top: 16px;
}

.buy b {
  color: #70462e;
  white-space: nowrap;
}

.small {
  padding: 9px 12px;
  font-size: 12px;
}

/* CART */
.cart-section {
  background: #f7efe8;
}

.cart-layout {
  display: grid;
  grid-template-columns: 1.8fr 1fr;
  gap: 28px;
  align-items: start;
}

.cart-items {
  display: flex;
  flex-direction: column;
  gap: 15px;
}

.empty-cart {
  background: white;
  padding: 50px 20px;
  text-align: center;
  border-radius: 12px;
}

.empty-cart span {
  font-size: 45px;
}

.empty-cart h3 {
  margin: 10px 0;
}

.empty-cart p {
  color: #88776d;
  margin-bottom: 20px;
}

.cart-item {
  background: white;
  padding: 17px;
  border-radius: 10px;
  display: flex;
  align-items: center;
  gap: 17px;
  box-shadow: 0 3px 12px #00000008;
}

.cart-item img {
  width: 95px;
  height: 95px;
  object-fit: cover;
  border-radius: 8px;
}

.cart-product-info {
  flex: 1;
}

.cart-product-info h3 {
  font-size: 16px;
}

.cart-product-info p {
  color: #947a68;
  font-size: 13px;
}

.cart-price {
  color: #70462e;
  font-weight: 700;
  margin-top: 5px;
}

.quantity {
  display: flex;
  align-items: center;
  gap: 12px;
  margin-top: 9px;
}

.quantity button {
  width: 27px;
  height: 27px;
  background: #f2e6dc;
  color: #70462e;
  border: none;
  border-radius: 5px;
  font-weight: bold;
}

.remove-btn {
  background: none;
  border: none;
  color: #c54c42;
  font-size: 13px;
  margin-top: 8px;
}

.bill-card {
  background: white;
  padding: 25px;
  border-radius: 12px;
  box-shadow: 0 4px 20px #0000000c;
  position: sticky;
  top: 100px;
}

.bill-card h3 {
  font-size: 21px;
  margin-bottom: 20px;
}

.bill-line {
  display: flex;
  justify-content: space-between;
  gap: 10px;
  margin: 14px 0;
  color: #76645a;
  font-size: 14px;
}

.bill-line span:last-child {
  text-align: right;
  font-weight: 600;
  color: #493024;
}

.bill-card hr,
.checkout-info hr {
  border: none;
  border-top: 1px solid #eee2d8;
  margin: 18px 0;
}

.bill-line.total {
  font-size: 19px;
  font-weight: 800;
  color: #493024;
}

.bill-line.total span:last-child {
  color: #70462e;
  font-size: 20px;
}

.offer-note {
  background: #f7efe8;
  color: #805334;
  padding: 12px;
  border-radius: 7px;
  font-size: 12px;
  margin: 18px 0;
}

.checkout-btn,
.place-order-btn {
  width: 100%;
  padding: 14px;
}

.checkout-btn:disabled {
  background: #b9aaa0;
  cursor: not-allowed;
  transform: none;
}

/* CHECKOUT */
.checkout-section {
  background: #fffaf5;
}

.checkout-layout {
  display: grid;
  grid-template-columns: 1.5fr 1fr;
  gap: 30px;
  align-items: start;
  max-width: 1000px;
  margin: auto;
}

.checkout-form,
.checkout-info {
  background: white;
  padding: 30px;
  border-radius: 12px;
  box-shadow: 0 4px 20px #0000000b;
}

.checkout-form h3,
.checkout-info h3 {
  margin-bottom: 20px;
  color: #493024;
}

.checkout-form label:not(.payment-option) {
  display: block;
  font-weight: 600;
  font-size: 14px;
  margin: 14px 0 6px;
}

.checkout-form input:not([type="radio"]),
.checkout-form textarea {
  width: 100%;
  padding: 12px;
  border: 1px solid #e4d7cd;
  border-radius: 6px;
  background: #fffdfb;
  outline: none;
}

.checkout-form input:focus,
.checkout-form textarea:focus {
  border-color: #a36b45;
  box-shadow: 0 0 0 3px #a36b4518;
}

.checkout-form textarea {
  resize: vertical;
}

.payment-option {
  display: flex;
  align-items: center;
  gap: 10px;
  padding: 12px;
  margin: 8px 0;
  background: #faf5f0;
  border-radius: 7px;
  cursor: pointer;
}

.payment-option input {
  accent-color: #70462e;
}

.checkout-info p {
  margin: 15px 0;
  color: #76645a;
  font-size: 14px;
}

/* ORDER SUCCESS */
.success-section {
  text-align: center;
}

.success-card {
  max-width: 600px;
  margin: auto;
  padding: 40px;
  background: white;
  border-radius: 15px;
  box-shadow: 0 5px 25px #00000010;
}

.success-icon {
  width: 65px;
  height: 65px;
  border-radius: 50%;
  background: #e3f3df;
  color: #38843a;
  font-size: 38px;
  margin: 0 auto 20px;
}

.success-card h2 {
  color: #38843a;
}

.success-card > p {
  color: #76645a;
  margin: 15px 0;
}

.order-details {
  background: #faf5f0;
  padding: 20px;
  text-align: left;
  border-radius: 8px;
  margin: 25px 0;
}

.order-details p {
  margin: 9px 0;
}

/* CTA */
.cta {
  background: #70462e;
  color: white;
  text-align: center;
  padding: 50px 20px;
}

.cta h2 {
  font-size: 30px;
}

.cta p {
  margin: 10px 0 20px;
  color: #f0ded0;
}

.cta .btn {
  background: white;
  color: #70462e;
}

/* FOOTER */
footer {
  background: #2e201a;
  color: white;
  padding: 45px 8% 20px;
}

.footer-top {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 30px;
  padding-bottom: 30px;
}

.footer-col h4 {
  margin-bottom: 15px;
  font-size: 18px;
}

.footer-col p,
.footer-col a {
  display: block;
  color: #d1bfb2;
  font-size: 14px;
  margin: 7px 0;
}

.footer-col a:hover {
  color: white;
}

.footer-bottom {
  border-top: 1px solid #59453a;
  padding-top: 20px;
  text-align: center;
  color: #d1bfb2;
  font-size: 13px;
}

[hidden] {
  display: none !important;
}

/* RESPONSIVE DESIGN */
@media (max-width: 900px) {
  .products {
    grid-template-columns: repeat(2, 1fr);
  }

  .cart-layout,
  .checkout-layout {
    grid-template-columns: 1fr;
  }

  .bill-card {
    position: static;
  }
}

@media (max-width: 600px) {
  .navbar {
    padding: 14px 5%;
    flex-wrap: wrap;
    gap: 12px;
  }

  .nav-links {
    order: 3;
    width: 100%;
    justify-content: center;
    gap: 15px;
    font-size: 13px;
  }

  .hero {
    flex-direction: column;
    padding: 45px 6%;
  }

  .hero-photo img {
    height: 260px;
  }

  .features {
    grid-template-columns: 1fr;
  }

  .section {
    padding: 45px 5%;
  }

  .products {
    grid-template-columns: 1fr;
  }

  .cart-item {
    flex-wrap: wrap;
  }

  .cart-item img {
    width: 75px;
    height: 75px;
  }

  .checkout-form,
  .checkout-info {
    padding: 20px;
  }

  .footer-top {
    grid-template-columns: 1fr;
  }

  .cta h2 {
    font-size: 24px;
  }
}

```

## OUTPUT
<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/7cb3deea-6378-49cc-83c9-afc6fe4e54e2" />

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/2a53cb0e-d797-4ca9-8947-3c3463945137" />

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/63da2f5b-9372-4d40-83aa-e930b135d745" />

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/f8d1c877-021a-426a-a49b-4820f272e3f9" />

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/576a3ecc-2f75-4579-a9e5-8bb279ddc1b1" />

## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
