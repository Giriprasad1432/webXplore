# Total CSS Codes

## `index.css`
```css
/* 1. Basic Page Reset */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: Arial, Helvetica, sans-serif;
  background-color: #ffffff;
  color: #222222;
}

/* 3. Hero Section */
.Home {
  display: flex;
  flex-direction: column;
}

.hero {
  display: flex;
  flex-direction: column;
  justify-content: center;

  gap: 15px;
  padding: 0 200px;

  width: 100%;
  height: calc(100vh - 80px);
  min-height: 600px;

  background:
    linear-gradient(rgba(32, 25, 25, 0.45), rgba(26, 18, 18, 0.45)),
    url("images/bg.jpeg");

  background-size: cover;
  background-repeat: no-repeat;
  background-position: center;
}

.button {
  display: inline-block;
  width: 130px;

  padding: 10px;

  background-color: rgb(128, 62, 44);
  color: white;

  text-decoration: none;
  text-align: center;

  border-radius: 8px;
  font-size: 16px;
  font-weight: bold;

  border: none;
  cursor: pointer;
  height: 35px;
}
.button a {
  text-decoration: none;
  color: white;
}
.hero h1 {
  font-size: 25px;
  margin: 0;
  color: rgb(128, 62, 44);
}

.hero h2 {
  margin: 0;

  font-size: 50px;
}

.hero h2 span {
  color: rgb(128, 62, 44);
}

.hero p {
  padding: 0;
  margin: 0;
  color: rgb(16, 16, 16);
  font-size: 18px;
}

/* 4. Featured Categories Section */
.cat {
  display: flex;
  flex-direction: column;
  gap: 20px;
  
  background: linear-gradient(to bottom, rgb(243, 248, 251), rgb(181, 221, 240));
  padding: 30px 20px;
  margin-bottom: 40px;
}

.cat h2 {
  text-align: center;
  font-size: 26px;
}

.cat-cards {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: center;
  gap: 25px;
}

.cat-card {
  width: 170px;
  height: 180px;
  background-color: #ffffff;
  border-radius: 20px;
  display: flex;
  flex-direction: column;
  text-align: center;
  justify-content: center;
  align-items: center;
  gap: 12px;
  padding: 10px;
  text-decoration: none;
  color: #222;
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.05);
  transition: transform 0.3s ease;
}

.cat-card:hover {
  transform: scale(1.08);
}

.cat-card img {
  width: 90px;
  height: 90px;
  object-fit: contain;
  border-radius: 12px;
}

.cat-card h4 {
  margin: 0;
  font-size: 15px;
}

/* 5. Featured Products Section */
.deals {
  display: flex;
  flex-direction: column;
  gap: 20px;
  background: linear-gradient(to right, rgb(236, 233, 236), rgb(213, 198, 209));
  padding: 30px 20px;
  margin-bottom: 40px;
}

.deals h2 {
  text-align: center;
  font-size: 26px;
}

.deals-cards {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: center;
  gap: 25px;
}

.deals-card {
  width: 200px;
  background-color: #ffffff;
  border-radius: 20px;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-items: center;
  padding: 15px;
  text-align: center;
  gap: 12px;
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.05);
  transition: transform 0.3s ease;
}

.deals-card:hover {
  transform: scale(1.08);
}

.deals-card img {
  width: 140px;
  height: 140px;
  object-fit: contain;
  border-radius: 20px;
}

.deals-card h4 {
  margin: 0;
  font-size: 16px;
}

.deals-card p {
  margin: 5px 0 0 0;
  font-weight: bold;
  color: #f47b20;
}
```

## `products.css`
```css
* {
    margin: 0;
    padding: 0;
}

body {
    font-family: Arial, Helvetica, sans-serif;
    background: #ffffff;
    color: #222;
}

main {
    padding: 20px 50px 30px;
}

.products-header {
    text-align: center;
    margin-bottom: 30px;
}

.products-header h1 {
    font-size: 32px;
    margin-bottom: 10px;
    color: #111;
}

.products-header p {
    font-size: 15px;
    color: #777;
}

.filters {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 30px;
    gap: 20px;
}

.categories {
    display: flex;
    gap: 8px;
    flex-wrap: wrap;
}

.categories button {
    border: 1px solid #e5e5e5;
    background: #fff;
    padding: 8px 14px;
    border-radius: 20px;
    font-size: 12px;
    cursor: pointer;
}

.categories button:hover,
.categories .selected {
    background: #f47b20;
    color: white;
    border-color: #f47b20;
}

.sort {
    display: flex;
    align-items: center;
    gap: 8px;
    white-space: nowrap;
}

.sort select {
    padding: 6px 10px;
    border: 1px solid #ddd;
    border-radius: 5px;
    font-size: 13px;
    outline: none;
}

.product-grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 25px;
}

.product-card {
    background: #fff;
    border: 1px solid #eee;
    border-radius: 12px;
    padding: 20px;
    text-align: center;
    transition: 0.3s;
    box-shadow: 0 4px 10px rgba(0, 0, 0, 0.05);
}

.product-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 8px 20px rgba(0, 0, 0, 0.1);
}

.product-card img {
    width: 100%;
    height: 180px;
    object-fit: contain;
    margin-bottom: 15px;
}

.product-card h3 {
    font-size: 16px;
    color: #333;
    margin-bottom: 8px;
}

.rating {
    color: #f47b20;
    font-size: 13px;
    margin-bottom: 8px;
}

.rating span {
    color: #888;
}

.price {
    font-size: 18px;
    font-weight: bold;
    color: #111;
    margin-bottom: 15px;
}

.price del {
    font-size: 14px;
    color: #999;
    font-weight: normal;
    margin-left: 5px;
}

.cart-btn {
    width: 100%;
    padding: 10px;
    background-color: #222;
    color: white;
    border: none;
    border-radius: 6px;
    font-size: 14px;
    font-weight: bold;
    cursor: pointer;
    transition: 0.3s;
}

.cart-btn:hover {
    background-color: #f47b20;
}

@media (max-width: 1024px) {
    .product-grid {
        grid-template-columns: repeat(3, 1fr);
    }
}

@media (max-width: 768px) {
    .product-grid {
        grid-template-columns: repeat(2, 1fr);
    }

    .filters {
        flex-direction: column;
        align-items: flex-start;
    }
}

@media (max-width: 480px) {
    .product-grid {
        grid-template-columns: 1fr;
    }
}
```

## `reviews.css`
```css
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    background-color: #ffffff;
    color: #222;
}

.reviews {
    text-align: center;
    padding: 55px 7% 70px;
}

.subtitle {
    color: #777;
    font-size: 15px;
    margin-bottom: 35px;
}

.review-container {
    display: flex;
    justify-content: center;
    gap: 25px;
    max-width: 1100px;
    margin: auto;
    flex-wrap: wrap;
}

.review-card {
    flex: 1 1 300px;
    max-width: 350px;
    padding: 25px;
    text-align: left;
    border: 1px solid #eee;
    border-radius: 10px;
    box-shadow: 0 3px 12px rgba(0, 0, 0, 0.06);
    background-color: white;
}

.customer {
    display: flex;
    align-items: center;
    gap: 15px;
    margin-bottom: 20px;
}

.customer img {
    border-radius: 50%;
}

.customer h3 {
    font-size: 15px;
    margin-bottom: 5px;
}

.stars {
    color: #f5a623;
    font-size: 14px;
}

.review-card p {
    color: #555;
    font-size: 14px;
    line-height: 1.7;
}

.review-button {
    margin-top: 30px;
    padding: 12px 25px;
    border: none;
    border-radius: 5px;
    background-color: #f47b20;
    color: white;
    cursor: pointer;
    font-size: 14px;
    font-weight: bold;
    transition: 0.3s;
}

.review-button:hover {
    background-color: #d96112;
}
```

## `contact.css`
```css
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, Helvetica, sans-serif;
    background: #ffffff;
    color: #222;
}

.contact-header {
    text-align: center;
    margin-bottom: 30px;
    padding: 0 20px;
}

.container {
    display: grid;
    grid-template-columns: 1.4fr 0.8fr;
    gap: 30px;
    max-width: 1100px;
    width: 100%;
    margin: 0 auto 40px auto;
    padding: 0 20px;
}

.contact,
.help {
    background: #fff;
    border: 1px solid #e5e5e5;
    border-radius: 12px;
    padding: 30px;
    box-shadow: 0 3px 12px rgba(0, 0, 0, 0.04);
}

.contact form {
    width: 100%;
}

.contact label {
    font-weight: 600;
    font-size: 16px;
    margin-bottom: 7px;
    display: inline-block;
}

.contact input,
.contact textarea {
    padding: 12px;
    margin-bottom: 18px;
    width: 100%;
    display: block;
    margin-top: 4px;
    border: 1px solid #ddd;
    border-radius: 6px;
    font-size: 15px;
    outline: none;
    background: #fcfcfc;
}

.contact input:focus,
.contact textarea:focus {
    border-color: #f47b20;
    background: #fff;
}

.contact button {
    background-color: #f47b20;
    color: white;
    padding: 10px 24px;
    border: none;
    border-radius: 6px;
    font-size: 15px;
    font-weight: bold;
    cursor: pointer;
    transition: 0.3s;
}

.contact button:hover {
    background: #d96112;
}

.help {
    display: flex;
    flex-direction: column;
    gap: 14px;
}

.help span {
    display: block;
    padding: 17px;
    border: 1px solid #eee;
    border-radius: 8px;
    background: #fff;
    font-size: 14px;
    color: #666;
    line-height: 1.6;
}

.help h4 {
    font-size: 17px;
    color: #171717;
    margin-bottom: 3px;
}

/* Responsive breakpoint for smaller screens */
@media (max-width: 800px) {
    .container {
        grid-template-columns: 1fr;
    }
}
```
