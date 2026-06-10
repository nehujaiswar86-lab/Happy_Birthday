<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Happy Birthday Sumeer 🎂</title>

<style>
*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:Arial,sans-serif;
}

body{
background:linear-gradient(135deg,#0f172a,#1e293b);
color:white;
text-align:center;
overflow-x:hidden;
}

header{
padding:50px 20px;
}

h1{
font-size:3rem;
color:#ffd700;
}

.subtitle{
margin-top:10px;
font-size:1.2rem;
}

.card{
background:rgba(255,255,255,0.08);
margin:20px auto;
padding:25px;
width:90%;
max-width:900px;
border-radius:20px;
backdrop-filter:blur(10px);
}

#countdown{
font-size:2rem;
font-weight:bold;
color:#00ffcc;
margin-top:15px;
}

.gallery{
display:flex;
flex-wrap:wrap;
justify-content:center;
gap:20px;
margin-top:20px;
}

.gallery img{
width:280px;
height:380px;
object-fit:cover;
border-radius:20px;
border:3px solid white;
transition:0.4s;
}

.gallery img:hover{
transform:scale(1.05);
}

.timeline{
text-align:left;
line-height:2;
font-size:18px;
}

.message{
font-size:18px;
line-height:1.8;
}

.cake{
font-size:100px;
animation:bounce 2s infinite;
}

@keyframes bounce{
50%{
transform:translateY(-15px);
}
}

button{
padding:12px 25px;
border:none;
border-radius:30px;
font-size:18px;
cursor:pointer;
background:#ff4081;
color:white;
margin-top:15px;
}

footer{
padding:30px;
font-size:14px;
opacity:0.8;
}

.confetti{
position:fixed;
width:10px;
height:10px;
top:-10px;
animation:fall 5s linear infinite;
}

@keyframes fall{
to{
transform:translateY(110vh) rotate(720deg);
}
}
</style>
</head>

<body>

<header>
<h1>🎂 Happy Birthday Sumeer 🎂</h1>
<p class="subtitle">
A special birthday website made with lots of memories 💙
</p>
</header>

<div class="card">
<h2>⏳ Birthday Countdown</h2>
<div id="countdown"></div>
</div>

<div class="card">
<h2>📸 Memories Gallery</h2>

<div class="gallery">
<img src="photo1.jpg" alt="">
<img src="photo2.jpg" alt="">
</div>
</div>

<div class="card">
<h2>🕒 Our Timeline</h2>

<div class="timeline">
<p>❤️ <b>2018</b> - Hamari journey ka ek important phase.</p>

<p>🌟 <b>First Meeting</b> - Woh din hamesha special rahega jab hum pehli baar mile the.</p>

<p>💙 <b>2026</b> - Itne saalon ke baad bhi yaadein aur connection special hain.</p>
</div>
</div>

<div class="card">
<h2>🎂 Birthday Cake</h2>

<div class="cake">
🎂
</div>

<p>Happy 28th Birthday, Sumeer!</p>
</div>

<div class="card">
<h2>💌 A Message For You</h2>

<p class="message">

Happy Birthday Sumeer! 🎉

8+ saalon mein bahut kuch badla,
bahut kuch seekhne ko mila,
aur bahut si yaadein bani.

Har phase mein tum meri life ka
ek important hissa rahe ho.

Main dil se wish karta hoon ki tum
hamesha khush raho,
healthy raho,
aur jo bhi sapne tum dekhte ho
woh poore ho.

Thank you for all the memories,
conversations,
support,
and moments we've shared
over the years.

You're truly one of the best friends
I could ever ask for.

Happy Birthday once again Sumeer! 🌟🎂

</p>
</div>

<div class="card">
<h2>🎵 Birthday Song</h2>

<p>
Add your MP3 file as <b>birthday.mp3</b>
in the same folder.
</p>

<audio controls>
<source src="birthday.mp3" type="audio/mpeg">
</audio>
</div>

<footer>
Made with 💙 for Sumeer
</footer>

<script>
const birthday = new Date("June 11, 2026 00:00:00").getTime();

setInterval(() => {

const now = new Date().getTime();
const distance = birthday - now;

if(distance < 0){
document.getElementById("countdown").innerHTML =
"🎉 HAPPY BIRTHDAY SUMEER 🎉";
return;
}

const days =
Math.floor(distance / (1000*60*60*24));

const hours =
Math.floor((distance%(1000*60*60*24))
/(1000*60*60));

const minutes =
Math.floor((distance%(1000*60*60))
/(1000*60));

const seconds =
Math.floor((distance%(1000*60))
/1000);

document.getElementById("countdown").innerHTML =
days+"d "+hours+"h "+
minutes+"m "+seconds+"s";

},1000);


for(let i=0;i<80;i++){

let confetti =
document.createElement("div");

confetti.classList.add("confetti");

confetti.style.left =
Math.random()*100+"vw";

confetti.style.background =
`hsl(${Math.random()*360},
100%,50%)`;

confetti.style.animationDelay =
Math.random()*5+"s";

document.body.appendChild(confetti);
}
</script>

</body>
</html>
