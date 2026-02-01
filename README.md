<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Free Fire ID Seller | Official Store</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<style>
*{box-sizing:border-box}
body{margin:0;font-family:Arial;background:#0b0f1a;color:#fff}
a{text-decoration:none;color:inherit}

/* LOGIN */
#loginBox{
  max-width:360px;margin:80px auto;background:#141a2e;
  padding:20px;border-radius:14px;text-align:center
}
#loginBox input{
  width:92%;padding:10px;margin:8px 0;border-radius:8px;border:none
}
#loginBox button{
  width:45%;margin:6px;padding:10px;border:none;
  border-radius:8px;font-weight:bold;background:#ff9800;cursor:pointer
}
#msg{color:#ff9800;font-size:14px}

/* hide site before login */
body:not(.logged) header,
body:not(.logged) .main,
body:not(.logged) footer,
body:not(.logged) .whatsapp{display:none}

/* HEADER */
header{
  background:linear-gradient(90deg,#ff9800,#ff3d00);
  padding:15px;text-align:center;
  font-size:22px;font-weight:bold
}

/* HERO */
.hero{
  text-align:center;padding:35px 15px;
  background:radial-gradient(circle,#1a1f3c,#0b0f1a)
}
.hero h1{color:#ffcc00;margin:0}
.hero p{opacity:.85}

/* TRUST */
.trust{
  display:grid;
  grid-template-columns:repeat(auto-fit,minmax(120px,1fr));
  gap:10px;padding:20px;text-align:center
}
.trust div{
  background:#141a2e;padding:12px;border-radius:10px
}

/* MAIN */
.main{padding:10px}
.section{padding:25px}
h2{color:#ff9800}

/* PROFILE CARDS */
.cards{
  display:grid;
  grid-template-columns:repeat(auto-fit,minmax(260px,1fr));
  gap:20px
}
.card{
  background:#141a2e;border-radius:15px;
  overflow:hidden;box-shadow:0 0 15px rgba(0,0,0,.6)
}
.card img{
  width:100%;height:220px;object-fit:cover
}
.info{padding:15px}
.info h3{margin:5px 0;color:#ffcc00}
.info p{margin:4px 0;font-size:14px}
.price{color:#00ff9c;font-weight:bold}
.btn{
  margin-top:10px;width:100%;padding:10px;
  border:none;border-radius:8px;
  background:#ff9800;font-weight:bold;cursor:pointer
}

/* FULL PROFILE VIEW */
#profileView{
  display:none;position:fixed;top:0;left:0;
  width:100%;height:100%;
  background:#0b0f1a;overflow:auto;z-index:10
}
.p-head{
  background:linear-gradient(90deg,#ff9800,#ff3d00);
  padding:15px;text-align:center
}
.p-body{
  max-width:800px;margin:20px auto;padding:15px
}
.p-body img{
  width:100%;max-height:350px;
  object-fit:cover;border-radius:15px
}
.stats{
  display:grid;
  grid-template-columns:repeat(auto-fit,minmax(140px,1fr));
  gap:10px;margin-top:15px
}
.stat{
  background:#141a2e;padding:12px;
  border-radius:10px;text-align:center
}
.close{background:red}

/* CONTACT */
.contact a{
  display:block;color:#00ff9c;margin:6px 0
}

/* FLOAT WHATSAPP */
.whatsapp{
  position:fixed;bottom:20px;right:20px;
  background:#25D366;color:#fff;
  font-size:26px;padding:14px;border-radius:50%
}

footer{
  text-align:center;padding:15px;
  background:#0a0e18;font-size:14px
}
</style>
</head>

<body>

<!-- LOGIN -->
<div id="loginBox">
  <h2>🔐 Login / Register</h2>
  <input id="user" placeholder="Username">
  <input id="pass" type="password" placeholder="Password">
  <button onclick="register()">Register</button>
  <button onclick="login()">Login</button>
  <p id="msg"></p>
</div>

<header>🔥 FREE FIRE ID SELLER – OFFICIAL STORE 🔥</header>

<div class="hero">
  <h1>Premium Free Fire Accounts</h1>
  <p>Safe • Instant Delivery • Trusted Seller</p>
</div>

<div class="trust">
  <div>✅ 100% Secure</div>
  <div>⚡ Instant Delivery</div>
  <div>⭐ Trusted Seller</div>
  <div>🔒 Safe Login</div>
</div>

<div class="main">

<!-- PROFILES -->
<div class="section">
<h2>🔥 Available Accounts</h2>
<div class="cards">

<div class="card">
<img src="https://i.imgur.com/8QfQY0R.jpg">
<div class="info">
<h3>PRO FF ACCOUNT</h3>
<p>Level: 65 | Rank: Heroic</p>
<p>Diamonds: 1200+ | Outfits: 350+</p>
<p class="price">₹8,999</p>
<button class="btn" onclick="openProfile(
'https://i.imgur.com/8QfQY0R.jpg',
'PRO FF ACCOUNT','65','Heroic','1200+','350+','Elite Guild','₹8,999'
)">View Profile</button>
</div>
</div>

</div>
</div>

<!-- PAYMENT -->
<div class="section">
<h2>💳 Payment Methods</h2>
<p>UPI: PhonePe / Google Pay / Paytm</p>
<p>Payment ke baad screenshot WhatsApp par bheje</p>
</div>

<!-- CONTACT -->
<div class="section">
<h2>📞 Contact & Support</h2>
<div class="contact">
<a href="https://wa.me/916203001040" target="_blank">WhatsApp</a>
<a href="https://facebook.com" target="_blank">Facebook</a>
<a href="https://instagram.com" target="_blank">Instagram</a>
</div>
</div>

</div>

<!-- FULL PROFILE -->
<div id="profileView">
  <div class="p-head"><h2 id="pn"></h2></div>
  <div class="p-body">
    <img id="pi">
    <div class="stats">
      <div class="stat">Level<br><b id="pl"></b></div>
      <div class="stat">Rank<br><b id="pr"></b></div>
      <div class="stat">Diamonds<br><b id="pd"></b></div>
      <div class="stat">Outfits<br><b id="po"></b></div>
    </div>
    <p>Guild: <b id="pg"></b></p>
    <p>Price: <b id="pp"></b></p>
    <button class="btn close" onclick="closeProfile()">Close</button>
  </div>
</div>

<a class="whatsapp" href="https://wa.me/916203001040" target="_blank">💬</a>

<footer>© 2026 Free Fire ID Seller | All Rights Reserved</footer>

<script>
function register(){
 if(!user.value||!pass.value){msg.innerText="Fill details";return;}
 localStorage.setItem("ff_user",user.value);
 localStorage.setItem("ff_pass",pass.value);
 msg.innerText="Registered! Now login";
}
function login(){
 if(user.value===localStorage.getItem("ff_user") &&
    pass.value===localStorage.getItem("ff_pass")){
   document.body.classList.add("logged");
   loginBox.style.display="none";
 }else msg.innerText="Wrong details";
}
function openProfile(i,n,l,r,d,o,g,p){
 profileView.style.display="block";
 pi.src=i;pn.innerText=n;pl.innerText=l;
 pr.innerText=r;pd.innerText=d;po.innerText=o;
 pg.innerText=g;pp.innerText=p;
}
function closeProfile(){profileView.style.display="none";}
</script>

</body>
</html>
