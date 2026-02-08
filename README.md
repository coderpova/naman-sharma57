# naman-sharma57
this is my 14th repository
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Flipkart Style Product Page</title>
    <style>
        :root {
            --fk-blue: #2874f0;
            --fk-yellow: #ff9f00;
            --fk-orange: #fb641b;
            --fk-bg: #f1f3f6;
            --fk-text: #212121;
        }

        body {
            font-family: Roboto, Arial, sans-serif;
            background-color: var(--fk-bg);
            margin: 0;
            color: var(--fk-text);
        }

        /* Top Header */
        header {
            background-color: var(--fk-blue);
            padding: 10px 0;
            display: flex;
            justify-content: center;
            position: sticky;
            top: 0;
            z-index: 100;
        }

        .header-container {
            width: 80%;
            display: flex;
            align-items: center;
            gap: 20px;
        }

        .logo { font-style: italic; color: white; font-weight: bold; font-size: 20px; }
        .search-bar { flex: 1; padding: 10px; border-radius: 2px; border: none; }

        /* Main Content */
        .container {
            display: grid;
            grid-template-columns: 40% 60%;
            background-color: white;
            width: 85%;
            margin: 20px auto;
            padding: 20px;
            box-shadow: 0 2px 4px rgba(0,0,0,0.1);
        }

        /* Image Column */
        .image-col { text-align: center; position: sticky; top: 80px; height: fit-content; }
        .product-img { width: 100%; max-width: 400px; padding: 10px; border: 1px solid #f0f0f0; }
        
        .button-group { display: flex; gap: 10px; margin-top: 20px; }
        .btn { flex: 1; padding: 18px; border: none; font-size: 16px; font-weight: bold; cursor: pointer; color: white; border-radius: 2px; }
        .add-to-cart { background-color: var(--fk-yellow); }
        .buy-now { background-color: var(--fk-orange); }

        /* Info Column */
        .info-col { padding: 0 30px; }
        .product-title { font-size: 18px; margin-bottom: 10px; }
        .rating-badge { background-color: #388e3c; color: white; padding: 2px 6px; border-radius: 3px; font-size: 12px; }
        .price { font-size: 28px; font-weight: bold; margin: 15px 0; }
        .offers { font-size: 14px; font-weight: bold; color: #388e3c; }
        
        .spec-list { list-style: none; padding: 0; font-size: 14px; line-height: 2; }
        .spec-list span { color: #878787; width: 100px; display: inline-block; }
    </style>
</head>
<body>

    <header>
        <div class="header-container">
            <div class="logo">Flipkart</div>
            <input type="text" class="search-bar" placeholder="Search for products, brands and more">
        </div>
    </header>

    <div class="container">
        <div class="image-col">
            <img src="https://m.media-amazon.com/images/I/61j6N9U1YGL._AC_SL1000_.jpg" class="product-img" alt="NE555 Timer IC">
            <div class="button-group">
                <button class="btn add-to-cart">🛒 ADD TO CART</button>
                <button class="btn buy-now">⚡ BUY NOW</button>
            </div>
        </div>

        <div class="info-col">
            <h1 class="product-title">NE555 Precision Timer IC Chips (Pack of 5) - For Electronics Projects & Engineering Labs</h1>
            <span class="rating-badge">4.9 ★</span> <span style="color:#878787; font-size:14px;">187 Ratings & 24 Reviews</span>
            
            <div class="price">₹75 <span style="text-decoration: line-through; color: #878787; font-size: 16px;">₹150</span> <span class="offers">50% off</span></div>
            
            <div style="font-weight: bold; margin-bottom: 10px;">Available offers</div>
            <div style="font-size: 14px; line-height: 1.8;">
                🏷️ <b>Bank Offer</b> 5% Cashback on Flipkart Axis Bank Card<br>
                🏷️ <b>Special Price</b> Get extra 10% off (price inclusive of cashback/coupon)
            </div>

            <h3 style="margin-top: 30px; border-bottom: 1px solid #f0f0f0; padding-bottom: 10px;">Specifications</h3>
            <ul class="spec-list">
                <li><span>Model Name</span> NE555 Precision Timer</li>
                <li><span>Type</span> Integrated Circuit (IC)</li>
                <li><span>Pins</span> 8-Pin DIP</li>
                <li><span>Package</span> Pack of 5</li>
            </ul>
        </div>
    </div>

</body>
</html>
