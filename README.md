MY MINJUU
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>17th Monthsary Surprise 💜</title>

<!-- Google Font -->
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Caveat:wght@400;500;600;700&family=Montserrat:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">

<style>

/* ==============================
   ROOT COLORS
============================== */

:root {
    --purple-dark: #12001f;
    --purple-deep: #21003b;
    --purple: #6c2bd9;
    --violet: #9b4dff;
    --lavender: #c084fc;
    --pink: #f0abfc;
    --white: #ffffff;
    --glass: rgba(255,255,255,0.09);
    --glass-border: rgba(255,255,255,0.18);
}

/* ==============================
   RESET
============================== */

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
}

body {
    font-family: "Montserrat", sans-serif;
    color: white;
    background:
        radial-gradient(circle at 20% 20%, rgba(155,77,255,.25), transparent 30%),
        radial-gradient(circle at 80% 30%, rgba(240,171,252,.18), transparent 30%),
        linear-gradient(135deg, #090014, #21003b 45%, #10001f);
    overflow-x: hidden;
}

/* ==============================
   LOADING SCREEN
============================== */

#loading {
    position: fixed;
    inset: 0;
    background: #090014;
    z-index: 99999;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    transition: 1s;
}

.loading-heart {
    font-size: 70px;
    animation: heartbeat 1s infinite;
}

#loading p {
    margin-top: 20px;
    font-size: 14px;
    letter-spacing: 4px;
    opacity: .7;
}

@keyframes heartbeat {
    0%,100% {
        transform: scale(1);
    }

    50% {
        transform: scale(1.25);
    }
}

/* ==============================
   PARTICLES
============================== */

#particles {
    position: fixed;
    inset: 0;
    pointer-events: none;
    z-index: 1;
}

.particle {
    position: absolute;
    width: 3px;
    height: 3px;
    background: white;
    border-radius: 50%;
    box-shadow: 0 0 12px white;
    animation: floatParticle linear infinite;
    opacity: .7;
}

@keyframes floatParticle {
    from {
        transform: translateY(110vh);
        opacity: 0;
    }

    20% {
        opacity: 1;
    }

    80% {
        opacity: .8;
    }

    to {
        transform: translateY(-10vh);
        opacity: 0;
    }
}

/* ==============================
   NAVIGATION
============================== */

nav {
    position: fixed;
    top: 20px;
    left: 50%;
    transform: translateX(-50%);
    width: min(90%, 850px);
    padding: 12px 22px;
    display: flex;
    justify-content: center;
    gap: 25px;
    z-index: 1000;

    background: rgba(25, 0, 45, .55);
    backdrop-filter: blur(18px);
    border: 1px solid var(--glass-border);
    border-radius: 50px;
    box-shadow: 0 10px 40px rgba(0,0,0,.3);
}

nav a {
    color: white;
    text-decoration: none;
    font-size: 12px;
    font-weight: 600;
    letter-spacing: 1px;
    transition: .3s;
}

nav a:hover {
    color: var(--pink);
    text-shadow: 0 0 15px var(--pink);
}

/* ==============================
   HERO
============================== */

.hero {
    min-height: 100vh;
    position: relative;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
    padding: 100px 20px 50px;
    z-index: 2;
}

.hero-content {
    max-width: 900px;
}

.small-title {
    letter-spacing: 7px;
    text-transform: uppercase;
    font-size: 13px;
    color: var(--pink);
    margin-bottom: 20px;
    animation: fadeUp 1.5s ease;
}

.hero h1 {
    font-family: "Caveat", cursive;
    font-size: clamp(70px, 12vw, 150px);
    line-height: .8;
    background: linear-gradient(
        90deg,
        #fff,
        #e9b5ff,
        #a855f7,
        #fff
    );
    background-size: 300%;
    -webkit-background-clip: text;
    color: transparent;
    animation:
        gradientText 5s infinite,
        fadeUp 1.5s ease;
    filter: drop-shadow(0 0 30px rgba(192,132,252,.5));
}

.hero h2 {
    font-size: clamp(20px, 4vw, 36px);
    margin-top: 30px;
    font-weight: 500;
    animation: fadeUp 2s ease;
}

.hero h2 span {
    color: var(--pink);
    font-weight: 700;
}

.hero-description {
    max-width: 600px;
    margin: 25px auto;
    line-height: 1.8;
    opacity: .75;
    animation: fadeUp 2.3s ease;
}

@keyframes gradientText {
    0% {
        background-position: 0%;
    }

    50% {
        background-position: 100%;
    }

    100% {
        background-position: 0%;
    }
}

@keyframes fadeUp {
    from {
        opacity: 0;
        transform: translateY(40px);
    }

    to {
        opacity: 1;
        transform: translateY(0);
    }
}

/* ==============================
   GLOWING HEART
============================== */

.big-heart {
    font-size: 65px;
    margin-top: 20px;
    animation: heartbeat 1.5s infinite;
    filter: drop-shadow(0 0 25px #d946ef);
}

/* ==============================
   BUTTON
============================== */

.btn {
    border: none;
    padding: 15px 30px;
    border-radius: 50px;
    color: white;
    background:
        linear-gradient(135deg, #7c3aed, #c026d3);
    font-weight: 700;
    letter-spacing: 1px;
    cursor: pointer;
    box-shadow:
        0 10px 30px rgba(124,58,237,.4),
        inset 0 0 15px rgba(255,255,255,.15);
    transition: .35s;
}

.btn:hover {
    transform: translateY(-5px) scale(1.04);
    box-shadow:
        0 15px 45px rgba(192,38,211,.6);
}

/* ==============================
   SECTIONS
============================== */

section {
    position: relative;
    z-index: 2;
    padding: 100px 20px;
}

.section-title {
    text-align: center;
    margin-bottom: 55px;
}

.section-title small {
    color: var(--pink);
    letter-spacing: 4px;
    text-transform: uppercase;
}

.section-title h2 {
    font-family: "Caveat", cursive;
    font-size: clamp(50px, 8vw, 80px);
    margin-top: 5px;
}

/* ==============================
   LOVE LETTER
============================== */

.letter-container {
    max-width: 850px;
    margin: auto;
    padding: 45px;
    border-radius: 30px;

    background:
        linear-gradient(
            135deg,
            rgba(255,255,255,.12),
            rgba(255,255,255,.04)
        );

    border: 1px solid var(--glass-border);
    backdrop-filter: blur(20px);

    box-shadow:
        0 30px 80px rgba(0,0,0,.3),
        inset 0 0 40px rgba(192,132,252,.05);

    position: relative;
}

.letter-container::before {
    content: "♡";
    position: absolute;
    top: -35px;
    right: 30px;
    font-size: 80px;
    color: rgba(240,171,252,.1);
}

.letter {
    font-family: "Caveat", cursive;
    font-size: 28px;
    line-height: 1.6;
}

.letter strong {
    color: var(--pink);
}

.signature {
    text-align: right;
    margin-top: 30px;
    font-size: 32px;
    color: var(--lavender);
}

/* ==============================
   COUNTER
============================== */

.counter-box {
    max-width: 850px;
    margin: auto;
    display: grid;
    grid-template-columns: repeat(4,1fr);
    gap: 15px;
}

.counter-item {
    padding: 25px 10px;
    text-align: center;

    border-radius: 20px;
    background: var(--glass);
    border: 1px solid var(--glass-border);
    backdrop-filter: blur(15px);
}

.counter-item span {
    display: block;
    font-size: 40px;
    font-weight: 800;
    background: linear-gradient(135deg,#fff,#d8b4fe);
    -webkit-background-clip: text;
    color: transparent;
}

.counter-item small {
    opacity: .6;
    letter-spacing: 2px;
}

/* ==============================
   REASONS
============================== */

.reasons {
    max-width: 1000px;
    margin: auto;

    display: grid;
    grid-template-columns: repeat(3,1fr);
    gap: 20px;
}

.reason-card {
    min-height: 210px;
    padding: 30px;
    border-radius: 25px;

    background:
        linear-gradient(
            145deg,
            rgba(255,255,255,.11),
            rgba(255,255,255,.035)
        );

    border: 1px solid rgba(255,255,255,.14);
    backdrop-filter: blur(15px);

    transition: .5s;
    overflow: hidden;
    position: relative;
}

.reason-card::after {
    content: "";
    position: absolute;
    width: 100px;
    height: 100px;
    background: #c026d3;
    filter: blur(70px);
    opacity: .25;
    right: -30px;
    bottom: -30px;
}

.reason-card:hover {
    transform: translateY(-10px) rotateX(4deg);
    border-color: rgba(240,171,252,.5);
    box-shadow: 0 20px 50px rgba(124,58,237,.25);
}

.reason-icon {
    font-size: 40px;
    margin-bottom: 20px;
}

.reason-card h3 {
    margin-bottom: 10px;
}

.reason-card p {
    font-size: 14px;
    line-height: 1.7;
    opacity: .65;
}

/* ==============================
   MEMORIES
============================== */

.memory-grid {
    max-width: 1000px;
    margin: auto;

    display: grid;
    grid-template-columns: repeat(3,1fr);
    gap: 20px;
}

.memory {
    height: 300px;
    border-radius: 25px;
    overflow: hidden;
    position: relative;

    background:
        linear-gradient(
            135deg,
            #6d28d9,
            #c026d3
        );

    border: 1px solid rgba(255,255,255,.2);
    transition: .5s;
}

.memory:hover {
    transform: scale(1.03);
    box-shadow: 0 25px 60px rgba(192,38,211,.35);
}

.memory-content {
    position: absolute;
    inset: 0;

    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;

    background:
        linear-gradient(
            transparent,
            rgba(0,0,0,.7)
        );

    text-align: center;
    padding: 20px;
}

.memory-icon {
    font-size: 65px;
    margin-bottom: 15px;
}

/* ==============================
   SURPRISE
============================== */

.surprise {
    min-height: 80vh;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
}

.surprise-box {
    max-width: 750px;
}

.surprise-box h2 {
    font-family: "Caveat", cursive;
    font-size: clamp(60px,10vw,100px);
    line-height: .9;
}

.surprise-box p {
    margin: 25px auto;
    max-width: 550px;
    line-height: 1.8;
    opacity: .7;
}

#surpriseMessage {
    display: none;
    margin-top: 40px;
    padding: 35px;
    border-radius: 25px;

    background: rgba(255,255,255,.08);
    border: 1px solid rgba(240,171,252,.3);

    animation: reveal .8s ease;
}

@keyframes reveal {
    from {
        opacity: 0;
        transform: scale(.7);
    }

    to {
        opacity: 1;
        transform: scale(1);
    }
}

/* ==============================
   FOOTER
============================== */

footer {
    position: relative;
    z-index: 2;
    text-align: center;
    padding: 50px 20px;
    border-top: 1px solid rgba(255,255,255,.1);
}

footer p {
    opacity: .5;
    font-size: 13px;
}

.footer-heart {
    font-size: 30px;
    margin-bottom: 15px;
}

/* ==============================
   FLOATING HEARTS
============================== */

.floating-heart {
    position: fixed;
    pointer-events: none;
    z-index: 999;
    animation: heartFloat 2s ease-out forwards;
}

@keyframes heartFloat {
    from {
        transform: translateY(0) scale(.5);
        opacity: 1;
    }

    to {
        transform: translateY(-150px) scale(1.5);
        opacity: 0;
    }
}

/* ==============================
   RESPONSIVE
============================== */

@media(max-width: 750px) {

    nav {
        gap: 12px;
        padding: 12px;
    }

    nav a {
        font-size: 9px;
    }

    .letter-container {
        padding: 30px 22px;
    }

    .letter {
        font-size: 23px;
    }

    .counter-box {
        grid-template-columns: repeat(2,1fr);
    }

    .reasons,
    .memory-grid {
        grid-template-columns: 1fr;
    }

    .memory {
        height: 260px;
    }
}

</style>
</head>

<body>

<!-- ==============================
     LOADING SCREEN
============================== -->

<div id="loading">
    <div class="loading-heart">💜</div>
    <p>Preparing something special...</p>
</div>

<!-- ==============================
     PARTICLES
============================== -->

<div id="particles"></div>

<!-- ==============================
     NAVIGATION
============================== -->

<nav>
    <a href="#home">HOME</a>
    <a href="#letter">LETTER</a>
    <a href="#reasons">WHY YOU</a>
    <a href="#memories">MEMORIES</a>
    <a href="#surprise">SURPRISE</a>
</nav>

<!-- ==============================
     HERO
============================== -->

<section class="hero" id="home">

    <div class="hero-content">

        <div class="small-title">
            A little surprise for my favorite person
        </div>

        <h1>17 Months</h1>

        <h2>
            of choosing <span>you</span> ❤️
        </h2>

        <p class="hero-description">
            Seventeen months of laughter, memories, little moments,
            random conversations, and countless reasons to be grateful
            that you came into my life.
        </p>

        <div class="big-heart">💜</div>

        <button class="btn" onclick="scrollToLetter()">
            Open My Heart ↓
        </button>

    </div>

</section>

<!-- ==============================
     LOVE LETTER
============================== -->

<section id="letter">

    <div class="section-title">

        <small>From my heart</small>

        <h2>A Letter For You</h2>

    </div>

    <div class="letter-container">

        <div class="letter">

            My love,

            <br><br>

            Happy <strong>17th Monthsary</strong> to us MY MINJUU LAB2. 💜

            <br><br>

            I honestly don't know how to put everything I feel
            into words, but I want you to know something simple:

            <strong>I am so grateful for you.</strong>

            <br><br>

            Thank you for every effort for me minjuu, for 
            every night talks with you my minjuu, i means a lot to me.
            Kabalo baka na Im very lucky to have you minjuu,
            ako gyud treasure every single time with you bisan sa VC ra minjuu,
            even in silent time minjuu and my ups and down, naa gihapon ka saakong side
            mao na very lucky kaayo ko nmo.
            I love you just the way you are minjuuu.

            <br><br>

            Seventeen months may sound like just a number,
            but for me, every month carries memories that
            I will always treasure. 

            <br><br>

            If I could choose again, I would still choose you.
            always minjuu, hehehehe syempreee.

            <br><br>

            And if I could make one wish for us maka laag2 nata minjuu,
            together, maka movie date nata  f2f maka eat nata sa mga favorite nato nga spots,
            maka travel together with youu.
            thats what i am wishing for us minjuu, and i hope soon we can make it happen .


            <br><br>

            You are one of the most beautiful chapters
            of my life.

            <br><br>

            <strong>
            Happy 17th Monthsary, my MINJUUU.. 💜
            </strong>

            <div class="signature">
                Forever yours,<br>
                ❤️ Your PAJIEE/PAJ2
            </div>

        </div>

    </div>

</section>

<!-- ==============================
     COUNTER
============================== -->

<section>

    <div class="section-title">

        <small>Our little milestone</small>

        <h2>17 Months Together</h2>

    </div>

    <div class="counter-box">

        <div class="counter-item">
            <span>17</span>
            <small>MONTHS</small>
        </div>

        <div class="counter-item">
            <span>∞</span>
            <small>MEMORIES</small>
        </div>

        <div class="counter-item">
            <span>1</span>
            <small>LOVE</small>
        </div>

        <div class="counter-item">
            <span>∞</span>
            <small>MORE TO COME</small>
        </div>

    </div>

</section>

<!-- ==============================
     REASONS
============================== -->

<section id="reasons">

    <div class="section-title">

        <small>There are so many...</small>

        <h2>Reasons I Love You</h2>

    </div>

    <div class="reasons">

        <div class="reason-card">

            <div class="reason-icon">🌷</div>

            <h3>Your Smile</h3>

            <p>
                Your smile has this magical way of making
                even an ordinary day feel special.
            </p>

        </div>

        <div class="reason-card">

            <div class="reason-icon">🫶</div>

            <h3>Your Heart</h3>

            <p>
                I love how caring, genuine, and beautiful
                your heart is.
            </p>

        </div>

        <div class="reason-card">

            <div class="reason-icon">😂</div>

            <h3>Your Laugh</h3>

            <p>
                Your laugh is one of those sounds I could
                listen to over and over again.
            </p>

        </div>

        <div class="reason-card">

            <div class="reason-icon">✨</div>

            <h3>Your Presence</h3>

            <p>
                Somehow, everything feels a little better
                whenever you're around even VC ra minjuu.
            </p>

        </div>

        <div class="reason-card">

            <div class="reason-icon">💫</div>

            <h3>Your Uniqueness</h3>

            <p>
                There is nobody quite like you, and that's
                exactly what makes you so special to me.
            </p>

        </div>

        <div class="reason-card">

            <div class="reason-icon">💜</div>

            <h3>Simply You</h3>

            <p>
                At the end of everything, I love you because
                you're you. And that's more than enough. i love just the way you are minjuu.
            </p>

        </div>

    </div>

</section>

<!-- ==============================
     MEMORIES
============================== -->

<section id="memories">

    <div class="section-title">

        <small>Our story</small>

        <h2>Little Memories</h2>

    </div>

    <div class="memory-grid">

        <div class="memory">

            <div class="memory-content">

                <div class="memory-icon">📸</div>

                <h3>Our First Memories</h3>

                <p>
                    The beginning of something beautiful.
                </p>

            </div>

        </div>

        <div class="memory">

            <div class="memory-content">

                <div class="memory-icon">🌙</div>

                <h3>Late Night Talks</h3>

                <p>
                    Conversations I never wanted to end.
                </p>

            </div>

        </div>

        <div class="memory">

            <div class="memory-content">

                <div class="memory-icon">💜</div>

                <h3>17 Months</h3>

                <p>
                    And somehow, I still want more.
                </p>

            </div>

        </div>

    </div>

</section>

<!-- ==============================
     SURPRISE
============================== -->

<section class="surprise" id="surprise">

    <div class="surprise-box">

        <div class="big-heart">💜</div>

        <h2>
            One Last<br>
            Surprise...
        </h2>

        <p>
            I made one final little message just for you.
            Don't press the button unless you're ready
            for something cheesy. 😌
        </p>

        <button class="btn" onclick="showSurprise()">
            🎁 Open Your Surprise
        </button>

        <div id="surpriseMessage">

            <h2 style="font-size:50px;">
                I LOVE YOU! 💜
            </h2>

            <p style="opacity:.9; margin-top:20px;">

                Happy 17th Monthsary, my MINJUUU.. 🥺💜

                <br><br>

                Thank you for being part of my life.

                <br>

                Thank you for staying.

                <br>

                Thank you for supporting me every time.

                <br><br>

                17 months down...

                <br>

                <strong>
                and hopefully forever to go. ♾️
                </strong>

                <br><br>

                No matter how many months pass,
                I hope we never stop choosing each other.

                <br><br>

                <span style="font-size:35px;">
                    💜 🫶 💍 ✨
                </span>

            </p>

        </div>

    </div>

</section>

<!-- ==============================
     FOOTER
============================== -->

<footer>

    <div class="footer-heart">💜</div>

    <p>
        Made with love for the most special girl in my world.
    </p>

    <p style="margin-top:10px;">
        Happy 17th Monthsary, my lab2 ✨
    </p>

</footer>

<script>

/* ==============================
   LOADING SCREEN
============================== */

window.addEventListener("load", function() {

    setTimeout(() => {

        document.getElementById("loading").style.opacity = "0";

        setTimeout(() => {

            document.getElementById("loading").style.display = "none";

        }, 1000);

    }, 1800);

});


/* ==============================
   PARTICLES
============================== */

const particleContainer =
    document.getElementById("particles");

for(let i = 0; i < 80; i++) {

    const particle =
        document.createElement("div");

    particle.className = "particle";

    particle.style.left =
        Math.random() * 100 + "%";

    particle.style.animationDuration =
        (5 + Math.random() * 10) + "s";

    particle.style.animationDelay =
        Math.random() * 10 + "s";

    particle.style.width =
        (1 + Math.random() * 4) + "px";

    particle.style.height =
        particle.style.width;

    particleContainer.appendChild(particle);
}


/* ==============================
   SCROLL BUTTON
============================== */

function scrollToLetter() {

    document.getElementById("letter")
        .scrollIntoView({
            behavior: "smooth"
        });

}


/* ==============================
   SURPRISE REVEAL
============================== */

function showSurprise() {

    const message =
        document.getElementById("surpriseMessage");

    message.style.display = "block";

    createHeartExplosion();

    setTimeout(() => {

        message.scrollIntoView({
            behavior: "smooth",
            block: "center"
        });

    }, 200);

}


/* ==============================
   HEART EXPLOSION
============================== */

function createHeartExplosion() {

    const hearts = [
        "💜",
        "💖",
        "💕",
        "💗",
        "✨",
        "💫",
        "🫶"
    ];

    for(let i = 0; i < 40; i++) {

        const heart =
            document.createElement("div");

        heart.className =
            "floating-heart";

        heart.innerHTML =
            hearts[Math.floor(Math.random() * hearts.length)];

        heart.style.left =
            (40 + Math.random() * 20) + "%";

        heart.style.top =
            (45 + Math.random() * 10) + "%";

        heart.style.fontSize =
            (15 + Math.random() * 25) + "px";

        heart.style.animationDuration =
            (1.5 + Math.random() * 2) + "s";

        document.body.appendChild(heart);

        setTimeout(() => {

            heart.remove();

        }, 3000);

    }

}


/* ==============================
   CLICK HEART EFFECT
============================== */

document.addEventListener("click", function(e) {

    if(
        e.target.tagName === "BUTTON" ||
        e.target.tagName === "A"
    ) return;

    const heart =
        document.createElement("div");

    heart.className =
        "floating-heart";

    heart.innerHTML = "💜";

    heart.style.left =
        e.clientX + "px";

    heart.style.top =
        e.clientY + "px";

    document.body.appendChild(heart);

    setTimeout(() => {

        heart.remove();

    }, 2000);

});


/* ==============================
   MOUSE GLOW
============================== */

document.addEventListener("mousemove", function(e) {

    document.body.style.background =
        `
        radial-gradient(
            circle at ${e.clientX}px ${e.clientY}px,
            rgba(155,77,255,.12),
            transparent 25%
        ),
        radial-gradient(
            circle at 20% 20%,
            rgba(155,77,255,.2),
            transparent 30%
        ),
        linear-gradient(
            135deg,
            #090014,
            #21003b 45%,
            #10001f
        )
        `;

});


/* ==============================
   CARD TILT EFFECT
============================== */

document.querySelectorAll(".reason-card")
.forEach(card => {

    card.addEventListener("mousemove", e => {

        const rect =
            card.getBoundingClientRect();

        const x =
            e.clientX - rect.left;

        const y =
            e.clientY - rect.top;

        const rotateX =
            ((y / rect.height) - .5) * -8;

        const rotateY =
            ((x / rect.width) - .5) * 8;

        card.style.transform =
            `perspective(700px)
             rotateX(${rotateX}deg)
             rotateY(${rotateY}deg)
             translateY(-8px)`;

    });

    card.addEventListener("mouseleave", () => {

        card.style.transform = "";

    });

});

</script>

</body>
</html>
```

