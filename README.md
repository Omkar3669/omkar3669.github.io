<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>BMW Luxury Cars & Bikes</title>

<link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@300;600&display=swap" rel="stylesheet">

<style>

*{
margin:0;
padding:0;
box-sizing:border-box;
font-family: 'Montserrat', sans-serif;
}

body{
background:#0a0a0a;
color:white;
}

header{
display:flex;
justify-content:space-between;
align-items:center;
padding:20px 60px;
background:black;
position:fixed;
width:100%;
z-index:1000;
}

.logo{
font-size:24px;
font-weight:600;
letter-spacing:2px;
}

nav a{
color:white;
margin-left:30px;
text-decoration:none;
font-weight:300;
}

.hero{
height:100vh;
background:url("https://images.unsplash.com/photo-1617531653332-bd46c24f2068") center/cover no-repeat;
display:flex;
align-items:center;
justify-content:center;
text-align:center;
}

.hero h1{
font-size:60px;
background:rgba(0,0,0,0.5);
padding:20px 40px;
}

.section{
padding:100px 60px;
}

.section h2{
text-align:center;
margin-bottom:50px;
font-size:40px;
}

.grid{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(280px,1fr));
gap:30px;
}

.card{
background:#111;
border-radius:10px;
overflow:hidden;
transition:0.4s;
}

.card:hover{
transform:scale(1.05);
box-shadow:0 10px 30px rgba(0,0,0,0.7);
}

.card img{
width:100%;
height:200px;
object-fit:cover;
}

.card h3{
padding:20px;
}

footer{
background:black;
text-align:center;
padding:30px;
margin-top:40px;
}

</style>

</head>

<body>

<header>

<div class="logo">BMW</div>

<nav>
<a href="#">Home</a>
<a href="#cars">Cars</a>
<a href="#bikes">Bikes</a>
<a href="#contact">Contact</a>
</nav>

</header>

<div class="hero">
<h1>Sheer Driving Pleasure</h1>
</div>

<section class="section" id="cars">

<h2>BMW Cars</h2>

<div class="grid">

<div class="card">
<img src="https://images.unsplash.com/photo-1503376780353-7e6692767b70">
<h3>BMW M4 Competition</h3>
</div>

<div class="card">
<img src="https://images.unsplash.com/photo-1555215695-3004980ad54e">
<h3>BMW i8</h3>
</div>

<div class="card">
<img src="https://images.unsplash.com/photo-1549924231-f129b911e442">
<h3>BMW X5</h3>
</div>

</div>

</section>

<section class="section" id="bikes">

<h2>BMW Motorcycles</h2>

<div class="grid">

<div class="card">
<img src="https://images.unsplash.com/photo-1558981285-6f0c94958bb6">
<h3>BMW S1000RR</h3>
</div>

<div class="card">
<img src="https://images.unsplash.com/photo-1609630875171-b1321377ee65">
<h3>BMW R1250GS</h3>
</div>

<div class="card">
<img src="https://images.unsplash.com/photo-1615172282427-9a57ef2d142e">
<h3>BMW G310R</h3>
</div>

</div>

</section>

<footer id="contact">

<p>Luxury BMW Showcase Website</p>
<p>© 2026 BMW Inspired Design</p>

</footer>

</body>
</html>
