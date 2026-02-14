# Birthday
wishing happy birthday
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Happy Birthday Jeevitha!</title>
  <style>
    body {
      margin: 0;
      font-family: 'Comic Sans MS', cursive, sans-serif;
      background: linear-gradient(135deg, #ff9a9e, #fad0c4);
      overflow: hidden;
      text-align: center;
      color: white;
    }

    h1 {
      margin-top: 40px;
      font-size: 3rem;
      animation: pop 1s ease-in-out infinite alternate;
      text-shadow: 2px 2px 8px rgba(0,0,0,0.3);
    }

    @keyframes pop {
      from { transform: scale(1); }
      to { transform: scale(1.1); }
    }

    .stage {
      position: relative;
      width: 100%;
      height: 70vh;
      display: flex;
      justify-content: center;
      align-items: flex-end;
      gap: 40px;
      padding-bottom: 40px;
    }

    .dog {
      font-size: 90px;
      animation: dance 1s infinite ease-in-out;
    }

    .dog:nth-child(2) { animation-delay: 0.2s; }
    .dog:nth-child(3) { animation-delay: 0.4s; }

    @keyframes dance {
      0%, 100% { transform: translateY(0) rotate(-5deg); }
      50% { transform: translateY(-40px) rotate(5deg); }
    }

    .drum {
      font-size: 40px;
      display: block;
      margin-top: -20px;
      animation: drumBeat 0.6s infinite;
    }

    @keyframes drumBeat {
      0%,100% { transform: scale(1); }
      50% { transform: scale(1.3); }
    }

    .confetti {
      position: fixed;
      top: -10px;
      width: 10px;
      height: 10px;
      background: yellow;
      animation: fall linear infinite;
    }

    @keyframes fall {
      to { transform: translateY(110vh) rotate(360deg); }
    }

    .footer {
      position: fixed;
      bottom: 10px;
      width: 100%;
      font-size: 18px;
      opacity: 0.9;
    }

    button {
      padding: 12px 24px;
      font-size: 18px;
      border: none;
      border-radius: 25px;
      background: #ff4081;
      color: white;
      cursor: pointer;
      box-shadow: 0 4px 12px rgba(0,0,0,0.3);
    }

    button:hover { transform: scale(1.05); }
  </style>
</head>
<body>

  <h1>🎉 Happy Birthday Jeevitha! 🎉</h1>

  <button onclick="startParty()">🎵 Tap to Start the Party 🎵</button>

  <div class="stage" id="stage" style="display:none;">
    <div class="dog">🐶<span class="drum">🥁</span></div>
    <div class="dog">🐶<span class="drum">🥁</span></div>
    <div class="dog">🐶<span class="drum">🥁</span></div>
  </div>

  <div class="footer">Made with ❤️ for Jeevitha</div>

  <audio id="music" loop>
    <source src="https://www2.cs.uic.edu/~i101/SoundFiles/HappyBirthday.mid" type="audio/midi">
  </audio>

  <script>
    function startParty() {
      document.getElementById('stage').style.display = 'flex';
      const music = document.getElementById('music');
      music.play();
      launchConfetti();
    }

    function launchConfetti() {
      for (let i = 0; i < 40; i++) {
        const conf = document.createElement('div');
        conf.className = 'confetti';
        conf.style.left = Math.random() * 100 + 'vw';
        conf.style.animationDuration = (Math.random() * 3 + 2) + 's';
        conf.style.background = `hsl(${Math.random()*360},100%,50%)`;
        document.body.appendChild(conf);
      }
    }
  </script>

</body>
</html>
