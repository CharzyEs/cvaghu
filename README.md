<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Our Little Love Story 🩵</title>

<style>
* {
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
}

body {
    margin: 0;
    font-family: 'Segoe UI', sans-serif;
    color: #527d9e;
    background: linear-gradient(
        180deg,
        #a8ddff 0%,
        #d6efff 45%,
        #f4fbff 100%
    );
    min-height: 100vh;
    overflow-x: hidden;
}

/* WALLPAPER */

.wallpaper {
    position: fixed;
    inset: 0;
    z-index: -2;
    overflow: hidden;
    pointer-events: none;
}

.cloud {
    position: absolute;
    width: 170px;
    height: 55px;
    background: white;
    border-radius: 100px;
    opacity: .65;
    filter: blur(2px);
    animation: cloudMove 18s linear infinite;
}

.cloud::before {
    content: "";
    position: absolute;
    width: 90px;
    height: 90px;
    background: white;
    border-radius: 50%;
    top: -40px;
    left: 35px;
}

.cloud::after {
    content: "";
    position: absolute;
    width: 70px;
    height: 70px;
    background: white;
    border-radius: 50%;
    top: -25px;
    right: 20px;
}

.c1 {
    top: 12%;
    left: -30%;
}

.c2 {
    top: 42%;
    left: -50%;
    animation-delay: -9s;
}

.c3 {
    top: 78%;
    left: -20%;
    animation-delay: -5s;
}

@keyframes cloudMove {
    from {
        transform: translateX(-200px);
    }

    to {
        transform: translateX(130vw);
    }
}

/* BINTANG */

.star {
    position: fixed;
    color: white;
    font-size: 22px;
    animation: sparkle 2s infinite alternate;
    pointer-events: none;
}

@keyframes sparkle {
    from {
        opacity: .2;
        transform: scale(.7);
    }

    to {
        opacity: 1;
        transform: scale(1.3);
    }
}

/* CONTAINER */

.container {
    width: 100%;
    max-width: 480px;
    margin: auto;
    padding: 35px 20px 60px;
    text-align: center;
}

/* CHARACTER */

.character {
    width: 230px;
    max-width: 90%;
    margin: 10px auto;
    animation: float 3s ease-in-out infinite;
    filter: drop-shadow(
        0 12px 15px rgba(80,150,200,.15)
    );
}

@keyframes float {
    0%,100% {
        transform: translateY(0);
    }

    50% {
        transform: translateY(-12px);
    }
}

h1 {
    color: #468fc5;
    font-size: 32px;
    margin: 15px 0;
    text-shadow: 2px 3px 0 #ffffff90;
}

.subtitle {
    font-size: 14px;
    line-height: 1.9;
    color: #648ca9;
}

/* CARD */

.card {
    margin-top: 28px;
    padding: 25px 20px;
    border-radius: 28px;
    background: rgba(255,255,255,.75);
    border: 2px solid white;
    box-shadow: 0 10px 30px rgba(91,164,210,.15);
    backdrop-filter: blur(12px);
}

.card h2 {
    color: #5a9dce;
    font-size: 20px;
}

/* TIMER */

.timer {
    display: flex;
    justify-content: space-between;
    gap: 8px;
    margin-top: 25px;
}

.time-box {
    flex: 1;
    background: #e8f6ff;
    border-radius: 16px;
    padding: 15px 3px;
    border: 1px solid white;
}

.number {
    font-size: 25px;
    font-weight: bold;
    color: #499bd3;
}

.label {
    font-size: 10px;
    margin-top: 5px;
    color: #83a8c2;
}

/* BUTTON */

button {
    border: none;
    border-radius: 30px;
    padding: 14px 25px;
    margin-top: 20px;
    background: linear-gradient(
        135deg,
        #8ccfff,
        #5aace9
    );
    color: white;
    font-size: 14px;
    font-weight: bold;
    box-shadow: 0 5px 15px rgba(70,150,220,.25);
    cursor: pointer;
    transition: .3s;
}

button:active {
    transform: scale(.94);
}

/* LETTER */

#letter {
    display: none;
    margin-top: 25px;
    text-align: left;
    line-height: 2;
    font-size: 14px;
    white-space: pre-line;
    color: #648ca9;
    animation: fadeIn .8s ease;
}

@keyframes fadeIn {
    from {
        opacity: 0;
        transform: translateY(20px);
    }

    to {
        opacity: 1;
        transform: translateY(0);
    }
}

/* FLOATING HEART */

.floating {
    position: fixed;
    bottom: -40px;
    pointer-events: none;
    z-index: 10;
    animation: rise linear forwards;
}

@keyframes rise {
    from {
        transform: translateY(0);
        opacity: 1;
    }

    to {
        transform: translateY(-110vh);
        opacity: 0;
    }
}

/* SETTINGS */

#settings {
    display: none;
    margin-top: 20px;
}

input, textarea {
    width: 100%;
    padding: 13px;
    margin-top: 12px;
    border-radius: 15px;
    border: 1px solid #b5def8;
    background: #f3faff;
    color: #527d9e;
    font-family: inherit;
}

textarea {
    height: 140px;
}

footer {
    margin-top: 40px;
    font-size: 12px;
    color: #79a9cb;
}
</style>
</head>

<body>

<!-- WALLPAPER -->

<div class="wallpaper">
    <div class="cloud c1"></div>
    <div class="cloud c2"></div>
    <div class="cloud c3"></div>
</div>

<div class="star" style="top:8%;left:12%">✦</div>
<div class="star" style="top:20%;right:10%">✧</div>
<div class="star" style="top:55%;left:8%">✦</div>
<div class="star" style="top:80%;right:15%">✧</div>

<div class="container">

    <p>☁️ OUR LITTLE LOVE STORY ☁️</p>

    <!-- KELINCI PUTIH -->

    <svg class="character"
    viewBox="0 0 300 230"
    xmlns="http://www.w3.org/2000/svg">

        <!-- TELINGA -->

        <ellipse
        cx="65" cy="100"
        rx="65" ry="27"
        fill="white"
        stroke="#c4e9ff"
        stroke-width="3"
        transform="rotate(-15 65 100)"/>

        <ellipse
        cx="235" cy="100"
        rx="65" ry="27"
        fill="white"
        stroke="#c4e9ff"
        stroke-width="3"
        transform="rotate(15 235 100)"/>

        <!-- KEPALA -->

        <ellipse
        cx="150" cy="115"
        rx="100" ry="85"
        fill="white"
        stroke="#c4e9ff"
        stroke-width="3"/>

        <!-- MATA -->

        <ellipse
        cx="115" cy="115"
        rx="7" ry="10"
        fill="#6c9bc3"/>

        <ellipse
        cx="185" cy="115"
        rx="7" ry="10"
        fill="#6c9bc3"/>

        <!-- PIPI -->

        <ellipse
        cx="95" cy="145"
        rx="17" ry="10"
        fill="#ffc8db"
        opacity=".8"/>

        <ellipse
        cx="205" cy="145"
        rx="17" ry="10"
        fill="#ffc8db"
        opacity=".8"/>

        <!-- MULUT -->

        <path
        d="M140 145 Q150 160 160 145"
        fill="none"
        stroke="#6c9bc3"
        stroke-width="4"
        stroke-linecap="round"/>

        <!-- PITA -->

        <path
        d="M125 45
        Q95 15 100 55
        Q105 75 130 60
        Q155 85 160 55
        Q165 20 135 45 Z"
        fill="#91d3ff"/>

        <circle
        cx="130" cy="52"
        r="10"
        fill="#5cafe8"/>

        <!-- BADAN -->

        <ellipse
        cx="150" cy="205"
        rx="45" ry="30"
        fill="white"
        stroke="#c4e9ff"
        stroke-width="3"/>

    </svg>

    <h1 id="title">
        Happy Anniversary! 🩵
    </h1>

    <p class="subtitle">
        Di antara banyaknya cerita,
        aku paling suka cerita tentang kita.
        <br><br>
        Terima kasih sudah menjadi
        bagian paling indah
        dalam hidupku.
        ☁️🤍
    </p>

    <!-- TIMER -->

    <div class="card">

        <h2>🩵 Our Time Together</h2>

        <p id="sinceDate"
        class="subtitle"></p>

        <div class="timer">

            <div class="time-box">
                <div class="number" id="days">0</div>
                <div class="label">HARI</div>
            </div>

            <div class="time-box">
                <div class="number" id="hours">0</div>
                <div class="label">JAM</div>
            </div>

            <div class="time-box">
                <div class="number" id="minutes">0</div>
                <div class="label">MENIT</div>
            </div>

            <div class="time-box">
                <div class="number" id="seconds">0</div>
                <div class="label">DETIK</div>
            </div>

        </div>

    </div>

    <!-- SURAT -->

    <div class="card">

        <h2>💌 A Letter For You</h2>

        <p class="subtitle">
            Aku punya sesuatu
            yang ingin kamu baca...
        </p>

        <button onclick="openLetter()">
            Open My Letter 💌
        </button>

        <div id="letter"></div>

    </div>

    <!-- KEJUTAN -->

    <div class="card">

        <h2>☁️ A Little Surprise</h2>

        <p class="subtitle">
            Kamu adalah alasan
            banyak senyum kecilku.
        </p>

        <button onclick="celebrate()">
            Tap Here! 🩵
        </button>

    </div>

    <!-- SETTINGS -->

    <div class="card">

        <h2>⚙️ Customize</h2>

        <button onclick="toggleSettings()">
            Edit Our Story
        </button>

        <div id="settings">

            <input
            id="nameInput"
            placeholder="Nama pasangan">

            <input
            type="date"
            id="dateInput">

            <textarea
            id="messageInput"
            placeholder="Surat cinta..."></textarea>

            <button onclick="saveSettings()">
                Save Changes 🩵
            </button>

        </div>

    </div>

    <footer>
        ☁️ Made with love ☁️
        <br>
        You & Me, Always. ♡
    </footer>

</div>

<script>

/* PENGATURAN AWAL */

let partnerName = "Sayang";

let anniversaryDate = "2025-10-20";

let loveMessage = `
Hai kamu! 🩵

Terima kasih sudah menjadi
bagian dari hidupku.

Aku senang sekali bisa
mengenalmu dan menjalani
hari-hari bersamamu.

Mungkin kita tidak selalu
punya hari yang sempurna.

Tapi aku ingin terus
menciptakan banyak kenangan
indah bersamamu.

Aku berharap kita bisa
terus saling menjaga,
saling memahami,
dan saling menyayangi.

Selamat merayakan
perjalanan kecil kita.

I love you,
today and always.

☁️🤍
`;

/* LOCAL STORAGE */

partnerName =
localStorage.getItem("cinnamonName")
|| partnerName;

anniversaryDate =
localStorage.getItem("cinnamonDate")
|| anniversaryDate;

loveMessage =
localStorage.getItem("cinnamonLetter")
|| loveMessage;

/* JUDUL */

function updateTitle() {

    document.getElementById("title")
    .textContent =
    "For " + partnerName + " 🩵";

}

/* TIMER */

function updateTimer() {

    const start =
    new Date(anniversaryDate + "T00:00:00");

    const diff =
    Math.max(0, Date.now() - start.getTime());

    const total =
    Math.floor(diff / 1000);

    document.getElementById("days")
    .textContent =
    Math.floor(total / 86400);

    document.getElementById("hours")
    .textContent =
    Math.floor((total % 86400) / 3600);

    document.getElementById("minutes")
    .textContent =
    Math.floor((total % 3600) / 60);

    document.getElementById("seconds")
    .textContent =
    total % 60;

    document.getElementById("sinceDate")
    .textContent =
    "Since " +
    start.toLocaleDateString(
        "id-ID",
        {
            day:"numeric",
            month:"long",
            year:"numeric"
        }
    );

}

/* SURAT */

function openLetter() {

    const letter =
    document.getElementById("letter");

    if(letter.style.display === "block") {

        letter.style.display = "none";

    } else {

        letter.textContent = loveMessage;

        letter.style.display = "block";

        createHearts(20);

    }

}

/* ANIMASI */

function createHearts(amount) {

    const symbols = [
        "🩵",
        "🤍",
        "☁️",
        "✨",
        "💙",
        "⭐"
    ];

    for(let i = 0; i < amount; i++) {

        const element =
        document.createElement("div");

        element.className = "floating";

        element.textContent =
        symbols[
            Math.floor(
                Math.random() * symbols.length
            )
        ];

        element.style.left =
        Math.random() * 100 + "vw";

        element.style.fontSize =
        (15 + Math.random() * 25) + "px";

        element.style.animationDuration =
        (3 + Math.random() * 4) + "s";

        document.body.appendChild(element);

        setTimeout(() => {
            element.remove();
        }, 7000);

    }

}

function celebrate() {
    createHearts(60);
}

/* SETTINGS */

function toggleSettings() {

    const settings =
    document.getElementById("settings");

    settings.style.display =
    settings.style.display === "block"
    ? "none"
    : "block";

    document.getElementById("nameInput")
    .value = partnerName;

    document.getElementById("dateInput")
    .value = anniversaryDate;

    document.getElementById("messageInput")
    .value = loveMessage;

}

function saveSettings() {

    partnerName =
    document.getElementById("nameInput")
    .value || "Sayang";

    anniversaryDate =
    document.getElementById("dateInput")
    .value || anniversaryDate;

    loveMessage =
    document.getElementById("messageInput")
    .value || loveMessage;

    localStorage.setItem(
        "cinnamonName",
        partnerName
    );

    localStorage.setItem(
        "cinnamonDate",
        anniversaryDate
    );

    localStorage.setItem(
        "cinnamonLetter",
        loveMessage
    );

    updateTitle();
    updateTimer();

    document.getElementById("settings")
    .style.display = "none";

    document.getElementById("letter")
    .style.display = "none";

    createHearts(30);

    alert("Saved successfully! 🩵");

}

/* START */

updateTitle();
updateTimer();

setInterval(updateTimer, 1000);

setInterval(() => {
    createHearts(1);
}, 3000);

</script>

</body>
</html># cvaghu