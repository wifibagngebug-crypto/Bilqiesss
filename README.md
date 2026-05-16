# Bilqiesss<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Untuk Cewek Cantik 💖</title>
<style>
    * {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
        font-family: 'Poppins', sans-serif;
    }

    body {
        background: linear-gradient(to bottom, #ffd6e7, #ffc0cb);
        text-align: center;
        color: #fff;
        overflow-x: hidden;
    }

    .container {
        padding: 30px;
    }

    .photo {
        width: 250px;
        height: 320px;
        object-fit: cover;
        border-radius: 20px;
        border: 5px solid white;
        box-shadow: 0 10px 30px rgba(0,0,0,0.2);
        margin-top: 20px;
    }

    h1 {
        margin-top: 20px;
        font-size: 32px;
        text-shadow: 2px 2px 10px rgba(0,0,0,0.2);
    }

    .text {
        margin-top: 25px;
        font-size: 18px;
        line-height: 1.8;
        background: rgba(255,255,255,0.2);
        padding: 20px;
        border-radius: 20px;
        backdrop-filter: blur(10px);
    }

    .love-btn {
        margin-top: 30px;
        padding: 15px 35px;
        border: none;
        border-radius: 30px;
        background: white;
        color: #ff4f8b;
        font-size: 18px;
        font-weight: bold;
        cursor: pointer;
        transition: 0.3s;
    }

    .love-btn:hover {
        transform: scale(1.08);
        background: #ffe6f0;
    }

    .popup {
        margin-top: 20px;
        font-size: 22px;
        font-weight: bold;
        color: white;
    }

    .heart {
        position: fixed;
        color: pink;
        font-size: 20px;
        animation: fall 5s linear infinite;
        top: -10px;
    }

    @keyframes fall {
        0% {
            transform: translateY(-10px);
            opacity: 1;
        }
        100% {
            transform: translateY(100vh);
            opacity: 0;
        }
    }
</style>
</head>
<body>

<div class="container">
    <img src="foto-cewek.jpg" alt="Foto Cantik" class="photo">

    <h1>Untuk Kamu yang Cantik 💕</h1>

    <div class="text">
        Kamu itu cantik, bukan cuma dari wajahmu, <br>
        tapi juga dari cara kamu tersenyum 🌸 <br><br>

        Matamu indah seperti bintang malam ✨ <br>
        Senyummu bisa bikin hari buruk jadi indah ☀️ <br>
        Kamu manis, lucu, dan selalu bikin kagum 💖 <br><br>

        Jujur aja... kamu itu tipe orang yang sekali dilihat,  
        susah untuk dilupakan 💗
    </div>

    <button class="love-btn" onclick="showLove()">
        Klik Kalau Kamu Cantik 💘
    </button>

    <div class="popup" id="popup"></div>
</div>

<script>
function showLove() {
    document.getElementById("popup").innerHTML =
        "Aku udah bilang kan? Kamu memang secantik itu 💞";
}

function createHeart() {
    const heart = document.createElement("div");
    heart.classList.add("heart");
    heart.innerHTML = "💖";
    heart.style.left = Math.random() * 100 + "vw";
    heart.style.fontSize = Math.random() * 20 + 15 + "px";
    document.body.appendChild(heart);

    setTimeout(() => {
        heart.remove();
    }, 5000);
}

setInterval(createHeart, 300);
</script>

</body>
</html>
