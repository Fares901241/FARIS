<!DOCTYPE html>
<html lang="ar">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>متجر الأزياء</title>
<link rel="stylesheet" href="styles.css">
</head>
<body>
<header>
    <nav>
        <ul>
            <li><a href="#home">الرئيسية</a></li>
            <li><a href="#about">عنا</a></li>
            <li><a href="#products">منتجاتنا</a></li>
            <li><a href="#contact">اتصل بنا</a></li>
        </ul>
    </nav>
</header>
<section id="home" class="hero">
    <h1>مرحباً بكم في عالم الأزياء</h1>
    <p>اكتشف أحدث التصاميم والعروض!</p>
</section>
<section id="products" class="product-gallery">
    <!-- المنتجات -->
    <article class="product">
        <img src="leather-jacket.jpg" alt="جاكيت جلدي">
        <div class="product-info">
            <h2>جاكيت جلدي</h2>
            <p>$299</p>
            <button>أضف إلى السلة</button>
        </div>
    </article>
    <!-- يمكن إضافة المزيด من المنتجات -->
</section>
<footer>
    <p>جميع الحقوق محفوظة &copy; 2024</p>
</footer>
<script src="scripts.js"></script>
</body>
</html>
body, html {
    margin: 0;
    padding: 0;
    font-family: 'Arial', sans-serif;
}
header nav ul {
    list-style: none;
    background: black;
    text-align: center;
    padding: 10px 0;
    margin: 0;
}
header nav ul li {
    display: inline;
}
header nav ul li a {
    text-decoration: none;
    color: white;
    padding: 15px 20px;
}
.hero {
    background: url('fashion-background.jpg') no-repeat center center/cover;
    color: white;
    text-align: center;
    padding: 100px 20px;
}
.product-gallery {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
    padding: 20px;
}
.product {
    margin: 10px;
    border: 1px solid #ccc;
    box-shadow: 2px 2px 8px #aaa;
}
.product img {
    width: 100%;
    height: auto;
}
.product-info {
    padding: 10px;
    text-align: center;
}
footer {
    background: black;
    color: white;
    text-align: center;
    padding: 10px;
// سكريبت بسيط لإضافة تفاعلية
document.addEventListener('DOMContentLoaded', function() {
    const buttons = document.querySelectorAll('.product button');
    buttons.forEach(button => {
        button.addEventListener('click', () => alert('تم إضافة المنتج إلى السلة!'));
    });
});
