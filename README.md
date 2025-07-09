# Product_card
## Date: 9/7/2025
## Objective:

To replicate a product card layout similar to those found on real-time e-commerce platform like FlipKart using the CSS Box Model (margin, border, padding, and content).

## Tasks:

#### 1. Structure the HTML Layout:
Create a container ```<div>``` for the product card.

Add an ```<img>``` for the product image.

Include ```<h2>``` for product name, ```<p>``` for description, and a ```<span>``` or ```<div>``` for price.

Add a “Buy Now” or “Add to Cart” button.

#### 2. Apply Box Model Styling in CSS:
Use padding inside each section (image, text, button) to ensure readability.

Use margin around the card to space it from the page edges or other cards.

Add a border to outline the card.

Control width and height for consistent sizing.

#### 3. Visual Styling:
Add a background color to the card container.

Use box-shadow to simulate depth (card lifting effect).

Add border-radius for rounded corners.

#### 4. Center the Card:
Use display: flex and justify-content: center and align-items: center on the parent container.

#### 5. Bonus Enhancements:
Use a hover effect on the button (e.g., background color change).

Make the card responsive with percentage-based widths or media queries.
## HTML Code:

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Flipkart Clone</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <div class="container">
    <div class="product-card">
      <img src="https://m.media-amazon.com/images/I/61HZLDc2ykL._AC_UY327_FMwebp_QL65_.jpg"  alt="Product" />
      <h2>Wireless Headphones</h2>
      <p>High-quality sound with long battery life. Lightweight and comfortable.</p>
      <span class="price">₹1,499</span>
      <button class="buy-btn">Add to Cart</button>
    </div>

    <div class="product-card">
      <img src="https://m.media-amazon.com/images/I/41Q+oC53k+L._SY300_SX300_.jpg" alt="Smartphone" />
      <h2>Redmi 12 5G</h2>
      <p>6.79-inch FHD+ display, Snapdragon 4 Gen 2, 5000mAh battery.</p>
      <span class="price">₹11,999</span>
      <button class="buy-btn">Add to Cart</button>
    </div>

    <div class="product-card">
      <img src="https://m.media-amazon.com/images/I/616rLWye9GL._SX522_.jpg" alt="Men's Watch" />
      <h2>Fastrack Men's Watch</h2>
      <p>Stylish analog watch with stainless steel strap and water resistance.</p>
      <span class="price">₹2,499</span>
      <button class="buy-btn">Add to Cart</button>
    </div>
  </div>
</body>
</html>

## CSS Code:


*{
    box-sizing: border-box;
}
body{
    margin: 0;
    background-color: #f2f2f2;
}
.container{
    height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 20px;
    
}
.product-card{
    background-color: #fff;
    border-radius: 10px;
    border: 1px solid #ddd;
    padding: 20px;
    margin: 20px;
    width: 280px;
    text-align: center;
    transition: transform 0.2s;
  box-shadow: 0 8px 16px rgba(0, 0, 0, 0.1);

}
.product-card:hover{
    transform: translateY(-5px);
}
.product-card img{
    width: 100%;
    height: auto;
    border-radius: 8px;
    margin-bottom: 15px;
}
.product-card h2{
    font-size: 25px;
    margin: 10px 0;
}

.product-card p {
  font-size: 16px;
  color: #555;
  margin: 10px 0;
}

.price {
  display: block;
  font-size: 20px;
  color: #388e3c;
  font-weight: bold;
  margin: 10px 0;
}

.buy-btn {
  padding: 10px 20px;
  background-color: #2874f0;
  color: white;
  border: none;
  border-radius: 5px;
  font-size: 15px;
  cursor: pointer;
  transition: background-color 0.3s ease;
}

.buy-btn:hover {
  background-color: #0f52ba;
}

## Output:
![Screenshot 2025-07-09 214041](https://github.com/user-attachments/assets/52a4d21a-992d-4a04-b9b2-c0f6d22f09e5)

## Result:
A product card layout similar to those found on real-time e-commerce platform like FlipKart using the CSS Box Model is replicated successfully.
