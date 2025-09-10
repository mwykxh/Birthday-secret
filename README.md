<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Happy Birthday Radha ❤️</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      font-family: 'Georgia', serif;
      background: linear-gradient(135deg, #ffdde1, #ee9ca7);
      color: #333;
      text-align: center;
      overflow-x: hidden;
    }
    h1 {
      font-size: 3rem;
      margin-top: 40px;
      color: #d63384;
      text-shadow: 2px 2px 8px rgba(0,0,0,0.2);
    }
    .letter {
      max-width: 800px;
      margin: 40px auto;
      padding: 20px 30px;
      background: rgba(255, 255, 255, 0.9);
      border-radius: 20px;
      box-shadow: 0px 8px 25px rgba(0,0,0,0.15);
      line-height: 1.8;
      font-size: 1.2rem;
      animation: fadeIn 3s ease-in-out;
    }
    .signature {
      margin-top: 30px;
      font-size: 1.5rem;
      color: #c1126b;
      font-style: italic;
    }
    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(50px); }
      to { opacity: 1; transform: translateY(0); }
    }
    /* Floating hearts */
    .heart {
      position: fixed;
      bottom: -10px;
      color: #ff4d6d;
      font-size: 20px;
      cursor: pointer;
      animation: floatUp 6s linear infinite;
    }
    @keyframes floatUp {
      0% { transform: translateY(0) rotate(0deg); opacity: 1; }
      100% { transform: translateY(-110vh) rotate(720deg); opacity: 0; }
    }
    /* Hidden surprise message */
    .popup {
      position: fixed;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      background: #fff0f6;
      padding: 25px 35px;
      border-radius: 20px;
      box-shadow: 0px 8px 25px rgba(0,0,0,0.25);
      font-size: 1.4rem;
      color: #d63384;
      display: none;
      animation: fadeIn 0.8s ease-in-out;
    }
  </style>
</head>
<body>

  <h1>🎉 Happy Birthday Radha (My Nani) ❤️</h1>

  <div class="letter">
    <p><b>My Dearest Radha (My Nani ❤️),</b></p>

    <p>On this beautiful day, <b>11th September 2009</b>, the world was blessed with someone truly special—you. From the moment you entered my life, everything changed. You became my reason to smile, my strength in every moment, and the most unforgettable part of my heart.</p>

    <p>Every memory with you feels like a chapter of the most beautiful love story ever written. The way you laugh, the way you care, the way you simply exist—it’s magic to me. I want you to know that no matter where life takes us, I will always hold this day close to my heart, because it gave me you.</p>

    <p>Radha, my Nani, you are not just my girlfriend—you are my best friend, my safe place, and my forever dream. I promise to love you endlessly, to stand by your side through every storm, and to celebrate every little moment of our lives together.</p>

    <p>Today is not just your birthday—it’s a reminder that love, destiny, and happiness are all real, because you are real. Thank you for being mine. Thank you for making me the happiest. Thank you for being you.</p>

    <p><b>Happy Birthday, my love. May this day be as unforgettable as our love. ❤️</b></p>

    <div class="signature">Forever and always yours,<br>💖 Kosu</div>
  </div>

  <!-- Hidden Surprise -->
  <div class="popup" id="popup">💖 I love you Nani ❤️ Forever yours, Kosu 💖</div>

  <!-- Background Music -->
  <audio autoplay loop>
    <source src="https://cdn.pixabay.com/download/audio/2022/03/15/audio_9a0462ec31.mp3?filename=romantic-piano-112194.mp3" type="audio/mp3">
  </audio>

  <script>
    // Create floating hearts
    function createHeart() {
      const heart = document.createElement("div");
      heart.className = "heart";
      heart.innerHTML = "❤";
      heart.style.left = Math.random() * 100 + "vw";
      heart.style.fontSize = Math.random() * 20 + 15 + "px";
      heart.style.animationDuration = Math.random() * 3 + 4 + "s";
      heart.onclick = () => {
        document.getElementById("popup").style.display = "block";
        setTimeout(() => {
          document.getElementById("popup").style.display = "none";
        }, 2500);
      };
      document.body.appendChild(heart);
      setTimeout(() => heart.remove(), 6000);
    }
    setInterval(createHeart, 400);
  </script>
</body>
</html>
