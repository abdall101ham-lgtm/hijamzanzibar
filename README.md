<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>Hijam Zanzibar Excursions & Safari</title>

<link rel="stylesheet"
href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css"/>

<style>

*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:Arial, sans-serif;
scroll-behavior:smooth;
}

:root{
--primary:#00b7b3;
--secondary:#ff9800;
--dark:#071414;
--white:#ffffff;
--light:#f3f8f8;
}

body{
background:var(--white);
color:#222;
overflow-x:hidden;
}

/* HEADER */

header{
position:fixed;
top:0;
width:100%;
padding:15px 8%;
display:flex;
justify-content:space-between;
align-items:center;
background:rgba(0,0,0,0.8);
backdrop-filter:blur(10px);
z-index:1000;
}

.logo{
display:flex;
align-items:center;
gap:10px;
}

.logo img{
width:70px;
height:70px;
border-radius:50%;
border:3px solid var(--primary);
object-fit:cover;
}

.logo h2{
color:white;
font-size:22px;
}

nav{
display:flex;
gap:25px;
}

nav a{
color:white;
text-decoration:none;
font-weight:bold;
transition:0.3s;
}

nav a:hover{
color:var(--secondary);
}

/* HERO */

.hero{
height:100vh;
background:
linear-gradient(rgba(0,0,0,0.6),rgba(0,0,0,0.6)),
url('https://images.unsplash.com/photo-1507525428034-b723cf961d3e');
background-size:cover;
background-position:center;
display:flex;
justify-content:center;
align-items:center;
text-align:center;
padding:20px;
color:white;
}

.hero-content{
max-width:850px;
}

.hero h1{
font-size:65px;
margin-bottom:20px;
}

.hero span{
color:var(--secondary);
}

.hero p{
font-size:22px;
line-height:1.7;
margin-bottom:35px;
}

.btn{
display:inline-block;
padding:15px 35px;
background:var(--primary);
color:white;
border-radius:40px;
text-decoration:none;
font-size:18px;
transition:0.3s;
}

.btn:hover{
background:var(--secondary);
transform:scale(1.05);
}

/* SECTION */

section{
padding:100px 8%;
}

.section-title{
text-align:center;
margin-bottom:60px;
}

.section-title h2{
font-size:45px;
color:var(--primary);
margin-bottom:15px;
}

/* ABOUT */

.about{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(320px,1fr));
gap:40px;
align-items:center;
}

.about img{
width:100%;
border-radius:20px;
height:450px;
object-fit:cover;
}

.about-text h3{
font-size:35px;
margin-bottom:20px;
color:var(--secondary);
}

.about-text p{
line-height:2;
font-size:18px;
}

/* TOURS */

.tours{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(280px,1fr));
gap:30px;
}

.card{
background:white;
border-radius:20px;
overflow:hidden;
box-shadow:0 5px 20px rgba(0,0,0,0.1);
transition:0.4s;
}

.card:hover{
transform:translateY(-10px);
}

.card img{
width:100%;
height:250px;
object-fit:cover;
}

.card-content{
padding:20px;
}

.card-content h3{
margin-bottom:10px;
color:var(--primary);
font-size:24px;
}

.card-content p{
line-height:1.7;
margin-bottom:15px;
}

.price{
font-size:22px;
font-weight:bold;
color:var(--secondary);
}

/* GALLERY */

.gallery{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
gap:20px;
}

.gallery img{
width:100%;
height:260px;
object-fit:cover;
border-radius:15px;
transition:0.4s;
cursor:pointer;
}

.gallery img:hover{
transform:scale(1.05);
}

/* BOOKING */

.booking{
background:var(--light);
border-radius:20px;
padding:50px;
}

.booking form{
display:grid;
gap:20px;
}

.booking input,
.booking textarea,
.booking select{
padding:15px;
border-radius:10px;
border:1px solid #ccc;
font-size:16px;
width:100%;
}

.booking button{
padding:15px;
background:var(--primary);
color:white;
border:none;
border-radius:10px;
font-size:18px;
cursor:pointer;
transition:0.3s;
}

.booking button:hover{
background:var(--secondary);
}

/* PAYMENT */

.payment{
background:var(--dark);
color:white;
padding:60px;
border-radius:20px;
text-align:center;
}

.payment h2{
font-size:40px;
margin-bottom:20px;
color:var(--secondary);
}

.payment p{
line-height:2;
font-size:18px;
}

/* CONTACT */

.contact{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(280px,1fr));
gap:30px;
margin-top:50px;
}

.contact-box{
background:white;
padding:30px;
border-radius:20px;
box-shadow:0 5px 20px rgba(0,0,0,0.1);
text-align:center;
}

.contact-box i{
font-size:40px;
color:var(--primary);
margin-bottom:20px;
}

.contact-box a{
text-decoration:none;
color:#222;
font-weight:bold;
}

/* FOOTER */

footer{
background:black;
color:white;
text-align:center;
padding:40px;
margin-top:60px;
}

.socials{
margin-top:20px;
display:flex;
justify-content:center;
gap:20px;
}

.socials a{
width:50px;
height:50px;
border-radius:50%;
display:flex;
justify-content:center;
align-items:center;
background:var(--primary);
color:white;
font-size:22px;
transition:0.3s;
text-decoration:none;
}

.socials a:hover{
background:var(--secondary);
transform:scale(1.1);
}

/* WHATSAPP */

.whatsapp{
position:fixed;
right:20px;
bottom:20px;
width:65px;
height:65px;
background:#25D366;
border-radius:50%;
display:flex;
justify-content:center;
align-items:center;
font-size:35px;
color:white;
text-decoration:none;
z-index:999;
box-shadow:0 5px 15px rgba(0,0,0,0.3);
}

/* RESPONSIVE */

@media(max-width:992px){

.hero h1{
font-size:50px;
}

}

@media(max-width:768px){

header{
flex-direction:column;
gap:15px;
}

nav{
flex-wrap:wrap;
justify-content:center;
}

.hero h1{
font-size:38px;
}

.hero p{
font-size:18px;
}

.section-title h2{
font-size:35px;
}

.about img{
height:350px;
}

}

@media(max-width:480px){

.hero{
padding-top:100px;
}

.hero h1{
font-size:30px;
}

.logo h2{
font-size:18px;
}

nav{
gap:12px;
}

nav a{
font-size:14px;
}

}

</style>
</head>

<body>

<!-- HEADER -->

<header>

<div class="logo">
<img src="4801.png" alt="Hijam Zanzibar Logo">
<h2>Hijam Zanzibar</h2>
</div>

<nav>
<a href="#home">Home</a>
<a href="#about">About</a>
<a href="#tours">Tours</a>
<a href="#gallery">Gallery</a>
<a href="#booking">Booking</a>
<a href="#contact">Contact</a>
</nav>

</header>

<!-- HERO -->

<section class="hero" id="home">

<div class="hero-content">

<h1>
Explore Beautiful
<span>Paje Zanzibar</span>
</h1>

<p>
Experience unforgettable beach holidays,
safari adventures, snorkeling, dolphin tours,
Stone Town tours and luxury excursions in Zanzibar.
</p>

<a href="#booking" class="btn">
Book Your Tour
</a>

</div>

</section>

<!-- ABOUT -->

<section id="about">

<div class="section-title">
<h2>About Company</h2>
</div>

<div class="about">

<img src="https://images.unsplash.com/photo-1540202404-a2f29016b523">

<div class="about-text">

<h3>Hijam Zanzibar Excursions & Safari</h3>

<p>
We are a professional Zanzibar tour company based near the
beautiful beaches of Paje Zanzibar. We organize unforgettable
excursions, snorkeling adventures, safari blue tours,
Mnemba dolphin trips, Stone Town tours and beach holidays.
Our goal is to give visitors the best Zanzibar experience
with comfort, safety and affordable prices.
</p>

</div>

</div>

</section>

<!-- TOURS -->

<section id="tours">

<div class="section-title">
<h2>Popular Tours</h2>
</div>

<div class="tours">

<div class="card">

<img src="https://images.unsplash.com/photo-1507525428034-b723cf961d3e">

<div class="card-content">

<h3>Paje Beach Tour</h3>

<p>
Enjoy white sand beaches and crystal clear ocean water.
</p>

<div class="price">$80</div>

</div>

</div>

<div class="card">

<img src="https://images.unsplash.com/photo-1518509562904-e7ef99cdcc86">

<div class="card-content">

<h3>Safari Blue</h3>

<p>
Ocean adventure with seafood lunch and snorkeling.
</p>

<div class="price">$120</div>

</div>

</div>

<div class="card">

<img src="https://images.unsplash.com/photo-1528127269322-539801943592">

<div class="card-content">

<h3>Mnemba Island</h3>

<p>
Swim with dolphins and discover coral reefs.
</p>

<div class="price">$150</div>

</div>

</div>

</div>

</section>

<!-- GALLERY -->

<section id="gallery">

<div class="section-title">
<h2>Tour Gallery</h2>
</div>

<div class="gallery">

<img src="https://images.unsplash.com/photo-1507525428034-b723cf961d3e">
<img src="https://images.unsplash.com/photo-1519046904884-53103b34b206">
<img src="https://images.unsplash.com/photo-1506744038136-46273834b3fb">
<img src="https://images.unsplash.com/photo-1528127269322-539801943592">
<img src="https://images.unsplash.com/photo-1518509562904-e7ef99cdcc86">
<img src="https://images.unsplash.com/photo-1540202404-a2f29016b523">

</div>

</section>

<!-- BOOKING -->

<section id="booking">

<div class="section-title">
<h2>Book Your Tour</h2>
</div>

<div class="booking">

<form id="bookingForm">

<input type="text"
placeholder="Your Full Name"
required>

<input type="email"
placeholder="Your Email"
required>

<input type="tel"
placeholder="Phone Number"
required>

<select required>

<option value="">
Select Tour Package
</option>

<option>
Paje Beach Tour
</option>

<option>
Safari Blue
</option>

<option>
Mnemba Island
</option>

<option>
Stone Town Tour
</option>

</select>

<input type="date" required>

<textarea rows="5"
placeholder="Additional Information">
</textarea>

<button type="submit">
Submit Booking
</button>

</form>

</div>

</section>

<!-- PAYMENT -->

<section>

<div class="payment">

<h2>Payment Methods</h2>

<p>
We accept secure online payments through:
</p>

<p>
M-Pesa • Airtel Money • Visa • Mastercard • PayPal
</p>

<p style="margin-top:20px;">
Fast and secure payment available 24/7.
</p>

</div>

</section>

<!-- CONTACT -->

<section id="contact">

<div class="section-title">
<h2>Contact Us</h2>
</div>

<div class="contact">

<div class="contact-box">

<i class="fa-solid fa-phone"></i>

<h3>Phone Number</h3>

<p>
<a href="tel:+255628232460">
+255 628 232 460
</a>
</p>

</div>

<div class="contact-box">

<i class="fa-brands fa-whatsapp"></i>

<h3>WhatsApp</h3>

<p>
<a href="https://wa.me/255628232460"
target="_blank">
Chat on WhatsApp
</a>
</p>

</div>

<div class="contact-box">

<i class="fa-solid fa-envelope"></i>

<h3>Email Address</h3>

<p>
<a href="mailto:abdall101ham@gmail.com">
abdall101ham@gmail.com
</a>
</p>

</div>

</div>

</section>

<!-- FOOTER -->

<footer>

<h2>Hijam Zanzibar Excursions & Safari</h2>

<p style="margin-top:15px;">
Paje Beach - Zanzibar Tanzania
</p>

<div class="socials">

<a href="https://vm.tiktok.com/ZS9Ytw5UfoXoa-K99xD/"
target="_blank">
<i class="fa-brands fa-tiktok"></i>
</a>

<a href="https://www.instagram.com/its_dream101?igsh=MW15bDRmYnludWNibA=="
target="_blank">
<i class="fa-brands fa-instagram"></i>
</a>

<a href="https://www.facebook.com/profile.php?id=100056204793312"
target="_blank">
<i class="fa-brands fa-facebook-f"></i>
</a>

</div>

<p style="margin-top:25px;">
© 2025 All Rights Reserved.
</p>

</footer>

<!-- WHATSAPP FLOAT -->

<a class="whatsapp"
href="https://wa.me/255628232460"
target="_blank">

<i class="fa-brands fa-whatsapp"></i>

</a>

<!-- JAVASCRIPT -->

<script>

document
.getElementById("bookingForm")
.addEventListener("submit", function(e){

e.preventDefault();

alert(
"Booking submitted successfully! We will contact you soon."
);

this.reset();

});

</script>

</body>
</html>
