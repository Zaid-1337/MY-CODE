# MY-CODE
MY E COOMERCE WEBSITE
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="css/style.css">

    <style>
 #box{
            background-color: rgb(224, 250, 215);
            height: 300px;
            width: 200px;
            display: none;
            position: absolute;
            left: 85%;
            top: 45%;
 }

    </style>
    
</head>
<body>
    <header class="navbar">
        <div class="logo">
            <h1>King Aamir</h1>
        </div>
        <nav>
            <ul>
                <li><a href="#">Home</a></li>
                <li><a href="#">Shop</a></li>
                <li><a href="#">Offers</a></li>
                <li id="pro"><a >Cart<span id="num">0</span></a></li>
                <li><a href="#">Login</a></li>
            </ul>
        </nav>

        <div id="box">

        </div>
    </header>

    
    <section class="hero">
        <div class="hero-content">
            <h2>Welcome To My Website</h2>
            <h3>WEB DEVLOPED BY AAMIR ALI</h3>
            <p>Your one-stop shop for all your needs</p>
            <button class="shop-now">Shop Now</button>
        </div>
    </section>

    
    <section class="products">
        <h2>Popular Products</h2>
        <div class="product-grid">
            <div class="product-card">
                <img src="download.jpg" alt="Product 1">
                <h3>Product 1</h3>
                <p>$20</p>
                
                <button class="btn">Add to Cart</button>
            </div>
            <div class="product-card">
                <img src="https://via.placeholder.com/200" alt="Product 2">
                <h3>Product 2</h3>
                <p>$30</p>
                <button class="btn">Add to Cart</button>
            </div>
            <div class="product-card">
                <img src="download.jpg" alt="">
                <h3>Product 3</h3>
                <p>$25</p>
                  <button class="btn">Add to Cart</button>
            </div>
            <div class="product-card">
                <img src="download.jpg" alt="">
                <h3>Product 3</h3>
                <p>$25</p>
                  <button class="btn">Add to Cart</button>
            </div>
        </div>
    </section>

    <footer>
        <p>&copy; 2025 Aamir.E. All Rights Reserved.</p>
    </footer>
    <script src="jquery-3.7.1.min.js"></script>

    <script>
        $(document).ready(function(){
                var count = 0;
                $('.btn').click(function(){
                    count++;
                    $('#num').html(count);
                });

                $('#pro').click(function(){
                    $('#box').slideToggle();
                });
        });
       

    </script>
    
</body>
</html>
