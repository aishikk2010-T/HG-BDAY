<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Happy Birthday HG(BABBYY) ❤️</title>

<style>

/* ======================================
   EASY CUSTOMIZATION SECTION
====================================== */

:root{
    --main-pink:#d8b4fe;
--light-pink:#f3e8ff;
--dark-pink:#a855f7;
--bg1:#faf5ff;
--bg2:#f3e8ff;
    --text:#5b3758;
}

/* ======================================
   GLOBAL
====================================== */

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}

html{
    scroll-behavior:smooth;
}

body{
    font-family:'Segoe UI',sans-serif;
    overflow-x:hidden;
    color:var(--text);
    background:linear-gradient(
    135deg,
    var(--bg1),
    var(--bg2)
    );
}

/* ======================================
   LOADER
====================================== */

#loader{
    position:fixed;
    inset:0;
    background:white;
    display:flex;
    justify-content:center;
    align-items:center;
    z-index:9999;
}

.loader-heart{
    font-size:60px;
    animation:pulse 1s infinite;
}

@keyframes pulse{
    50%{
        transform:scale(1.3);
    }
}

/* ======================================
   FLOATING HEARTS
====================================== */

.hearts{
    position:fixed;
    width:100%;
    height:100%;
    overflow:hidden;
    z-index:-1;
}

.heart{
    position:absolute;
    color:pink;
    animation:float 10s linear infinite;
    opacity:.6;
}

@keyframes float{
    from{
        transform:translateY(100vh);
    }
    to{
        transform:translateY(-100px);
    }
}

/* ======================================
   SPARKLES
====================================== */

.sparkle{
    position:fixed;
    width:4px;
    height:4px;
    background:white;
    border-radius:50%;
    box-shadow:0 0 10px white;
    animation:twinkle 2s infinite alternate;
}

@keyframes twinkle{
    from{opacity:.2;}
    to{opacity:1;}
}

/* ======================================
   LANDING
====================================== */

.hero{
    min-height:100vh;
    display:flex;
    flex-direction:column;
    justify-content:center;
    align-items:center;
    text-align:center;
    padding:20px;
}

.glow{
    font-size:4rem;
    color:var(--dark-pink);
    text-shadow:
    0 0 15px pink,
    0 0 30px hotpink;
    animation:fadeIn 2s ease;
}

.subtitle{
    margin-top:20px;
    font-size:1.3rem;
}

@keyframes fadeIn{
    from{
        opacity:0;
        transform:translateY(30px);
    }
    to{
        opacity:1;
        transform:translateY(0);
    }
}

/* ======================================
   SECTIONS
====================================== */

section{
    padding:80px 10%;
}

.card{
    background:rgba(255,255,255,.7);
    backdrop-filter:blur(10px);
    border-radius:25px;
    padding:30px;
    box-shadow:0 10px 40px rgba(255,105,180,.2);
}

/* ======================================
   GALLERY
====================================== */

.gallery{
    display:grid;
    grid-template-columns:
    repeat(auto-fit,minmax(220px,1fr));
    gap:20px;
}

.gallery img{
    width:100%;
    border-radius:20px;
    transition:.4s;
}

.gallery img:hover{
    transform:scale(1.05);
}

/* ======================================
   BUTTONS
====================================== */

.btn{
    padding:12px 25px;
    border:none;
    border-radius:30px;
    background:var(--dark-pink);
    color:white;
    cursor:pointer;
    transition:.3s;
}

.btn:hover{
    transform:translateY(-3px);
}

/* ======================================
   SURPRISE
====================================== */

.surprise{
    text-align:center;
}

.hidden{
    display:none;
}

.message{
    margin-top:25px;
    font-size:1.5rem;
    animation:fadeIn 1s ease;
}

/* ======================================
   FOOTER
====================================== */

footer{
    text-align:center;
    padding:40px;
}

/* ======================================
   MOBILE
====================================== */

@media(max-width:768px){

.glow{
    font-size:2.5rem;
}

.subtitle{
    font-size:1rem;
}

}

</style>
</head>
<body>

<!-- LOADER -->

<div id="loader">
    <div class="loader-heart">💖</div>
</div>

<!-- FLOATING HEARTS -->

<div class="hearts" id="hearts"></div>

<!-- SPARKLES -->

<div id="sparkles"></div>

<!-- MUSIC -->

<!-- REPLACE music.mp3 WITH YOUR FILE -->
<audio id="bgMusic" loop>
    <source src="Hareya hg.mp3" type="audio/mpeg">
</audio>

<!-- HERO -->

<section class="hero">

<h1 class="glow">
Happy Birthday ❤️
</h1>

<p class="subtitle">
To my bestest childhood friend ✨
</p>

<br>

<button class="btn" onclick="toggleMusic()">
🎵 Play / Pause Music
</button>

</section>

<!-- NOTE -->

<section>

<div class="card">

<h2>💌 A Special Note</h2>

<br>

<p>

<!-- REPLACE THIS MESSAGE -->

Happy Birthday to the most special person from my childhood.

Growing up with you is one of the best part of my life 
From silly conversations to bestest teas and all the memories we made together
Every moment still means a lot to me.No matter how much we grow up or how busy life gets 
You will always be my most important person i never forget.
Thanks for being there for me and you are the one who supported me a lot,
gave me emotional support when i need someone the most.
Am really lucky to have the bestest friend like you.
I just hope this year brings you success,happiness,peace and 
everything your heart wishes for cuz you truely deserve it all

Enjoy your day fully,smile a lot(MY CUTTIE PIE)
And Yeah.... Don't forget to send me snaps and fitchecks ❤️
And once again HAPPIEST BIRTHDAY TO YOU.

</p>

</div>

</section>

<!-- GALLERY -->

<section>

<div class="card">

<h2>📸 Our Memories</h2>

<br>

<div class="gallery">

<!-- REPLACE THESE WITH YOUR PHOTOS -->

<img src="HG photo2.jpeg">
<img src="Photo4.jpeg">
<img src="Photo3.jpeg">
<img src="Photo1.jpeg">
<img src="Photo5.jpeg">
<img src="Photo7.jpeg">

</div>

</div>

</section>

<!-- SURPRISE -->

<section>

<div class="card surprise">

<h2>🎁 Final Surprise</h2>

<br>

<button class="btn" onclick="showMessage()">
Click Me ❤️
</button>

<div id="surpriseMessage"
class="hidden message">

No matter how many birthdays pass,
you'll always remain one of the most
special people in my life.

Thank you for being part of my story.

Happy Birthday Princess 👑💖

</div>

</div>

</section>

<footer>
Made with ❤️ for my BABBYYY..
</footer>

<script>

/* ==========================
   LOADER
========================== */

window.onload = () => {
    setTimeout(()=>{
        document.getElementById("loader")
        .style.display="none";
    },1500);
};

/* ==========================
   MUSIC
========================== */

const music =
document.getElementById("bgMusic");

function toggleMusic(){

if(music.paused){
    music.play();
}else{
    music.pause();
}

}

/* ==========================
   SURPRISE
========================== */

function showMessage(){

document
.getElementById("surpriseMessage")
.classList.remove("hidden");

}

/* ==========================
   HEARTS
========================== */

const hearts =
document.getElementById("hearts");

for(let i=0;i<40;i++){

let heart =
document.createElement("div");

heart.className="heart";
heart.innerHTML="❤";

heart.style.left =
Math.random()*100+"vw";

heart.style.fontSize =
(Math.random()*20+10)+"px";

heart.style.animationDuration =
(Math.random()*10+5)+"s";

heart.style.opacity =
Math.random();

hearts.appendChild(heart);

}

/* ==========================
   SPARKLES
========================== */

for(let i=0;i<80;i++){

let sparkle =
document.createElement("div");

sparkle.className="sparkle";

sparkle.style.left =
Math.random()*100+"vw";

sparkle.style.top =
Math.random()*100+"vh";

sparkle.style.animationDelay =
Math.random()*2+"s";

document.body.appendChild(sparkle);

}

</script>

</body>
</html># index.html
