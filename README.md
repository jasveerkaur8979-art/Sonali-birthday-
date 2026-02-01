# Sonali-birthday-
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Happy Birthday Sonali 🎂</title>

<style>
body{
 margin:0;
 font-family:-apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
 background:#0e0e14;
 color:#fff;
 text-align:center;
 overflow-x:hidden;
}
h1{font-size:2.2rem; margin-top:30px}
p{color:#ddd}
.gallery{
 display:grid;
 grid-template-columns:repeat(auto-fit,minmax(140px,1fr));
 gap:12px;
 padding:20px;
}
.gallery img{
 width:100%;
 border-radius:16px;
}
.card{
 background:#151522;
 margin:20px;
 padding:24px;
 border-radius:22px;
}
.heart{
 position:fixed;
 bottom:-10px;
 animation:float 6s linear infinite;
 font-size:18px;
}
@keyframes float{
 from{transform:translateY(0);opacity:1}
 to{transform:translateY(-120vh);opacity:0}
}
.music{
 margin-top:15px;
 opacity:0.8;
}
</style>
</head>

<body>

<h1 id="type"></h1>
<p>6 February ✨</p>

<div class="music">
🎧 Zulfein for you 🤍
<audio controls autoplay loop>
  <source src="zulfein.mp3" type="audio/mpeg">
</audio>
</div>

<div class="gallery">
  <img src="photo1.jpg">
  <img src="photo2.jpg">
  <img src="photo3.jpg">
</div>

<div class="card">
<p>
Hey Sonali 🤍<br><br>
Tu sirf ek naam nahi hai,<br>
tu woh feeling hai jo har din ko special bana deti hai.
</p>

<p>
Teri hasi, teri baatein,<br>
aur teri zulfein…<br>
sab kuch bas dil me reh jaata hai.
</p>

<p>
Happy Birthday 🎂🤍<br>
Hamesha khush rehna.
</p>
</div>

<script>
const t="Happy Birthday Sonali 🎂🤍";
let i=0;
function type(){
 if(i<t.length){
  document.getElementById("type").innerHTML+=t.charAt(i);
  i++;
  setTimeout(type,90);
 }
}
type();

setInterval(()=>{
 let h=document.createElement("div");
 h.className="heart";
 h.style.left=Math.random()*100+"vw";
 h.innerHTML="🤍";
 document.body.appendChild(h);
 setTimeout(()=>h.remove(),6000);
},600);
</script>

</body>
</html>