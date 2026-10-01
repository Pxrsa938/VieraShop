<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>VieraShop</title>

<style>

*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:tahoma;
}

body{
background:#0b1120;
color:white;
}

header{
height:80px;
background:linear-gradient(90deg,#00bfff,#004cff);
display:flex;
justify-content:space-between;
align-items:center;
padding:0 40px;
box-shadow:0 0 30px #00bfff;
}

.logo{
font-size:30px;
font-weight:bold;
color:white;
}

nav button{
margin-right:10px;
padding:10px 20px;
border:none;
background:#0099ff;
color:white;
cursor:pointer;
}

.hero{
height:350px;
display:flex;
justify-content:center;
align-items:center;
flex-direction:column;
background:url("https://images.unsplash.com/photo-1627856014754-2907e2355d2d") center/cover;
}

.hero h1{
font-size:50px;
text-shadow:0 0 15px cyan;
}

.hero p{
margin-top:15px;
font-size:20px;
}

.products{
padding:50px;
display:grid;
grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
gap:25px;
}

.card{
background:#111827;
border:2px solid #00bfff;
padding:20px;
text-align:center;
transition:.3s;
}

.card:hover{
transform:translateY(-10px);
box-shadow:0 0 25px #00bfff;
}

.card img{
width:100%;
height:180px;
object-fit:cover;
}

.card h2{
margin-top:15px;
}

.price{
color:#00e5ff;
font-size:22px;
margin:15px;
}

.buy{
width:100%;
padding:12px;
border:none;
background:#00bfff;
color:white;
cursor:pointer;
font-size:18px;
}

footer{
padding:30px;
text-align:center;
background:#111;
margin-top:40px;
}

.alert{
position:fixed;
top:20px;
left:50%;
transform:translateX(-50%);
background:#00bfff;
padding:15px 40px;
display:none;
box-shadow:0 0 25px cyan;
font-size:18px;
}

</style>
</head>

<body>

<div class="alert" id="alert">
محصول به سبد خرید اضافه شد
</div>

<header>

<div class="logo">
VieraShop
</div>

<nav>

<button onclick="login()">
ورود
</button>

<button onclick="register()">
ساخت حساب
</button>

<button>
🛒 سبد خرید
</button>

</nav>

</header>

<section class="hero">

<h1>به VieraShop خوش آمدید</h1>

<p>بهترین فروشگاه محصولات Minecraft</p>

</section>

<section class="products">

<div class="card">

<img src="https://i.imgur.com/Tu5N5Vf.png">

<h2>OptiFine Cape</h2>

<div class="price">
26,000 تومان
</div>

<button class="buy" onclick="buy()">
+ افزودن به سبد خرید
</button>

</div>

<div class="card">

<img src="https://i.imgur.com/KhL0M6D.png">

<h2>Minecraft Premium</h2>

<div class="price">
2,500,000 تومان
</div>

<button class="buy" onclick="buy()">
+ افزودن به سبد خرید
</button>

</div>

<div class="card">

<img src="https://i.imgur.com/k5jL7UC.png">

<h2>Pixel Art</h2>

<div class="price">
5,000 تومان
</div>

<button class="buy" onclick="buy()">
+ افزودن به سبد خرید
</button>

</div>

</section>

<footer>

© 2026 VieraShop

</footer>

<script>

function buy(){

let a=document.getElementById("alert");

a.style.display="block";

setTimeout(function(){

a.style.display="none";

},2000);

}

function login(){

alert("سیستم ورود به زودی اضافه می‌شود.");

}

function register(){

alert("سیستم ساخت حساب به زودی اضافه می‌شود.");

}

</script>

</body>
</html>
