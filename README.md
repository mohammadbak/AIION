<!DOCTYPE html>
<html lang="fa">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>BNB AI Token 3D</title>
  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; }
    body {
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      font-family: Arial, sans-serif;
      background: linear-gradient(135deg, #0f2027, #203a43, #2c5364);
      overflow: hidden;
      perspective: 1000px; /* برای افکت 3D */
    }

    .hero {
      position: relative;
      text-align: center;
      transform-style: preserve-3d;
      transition: transform 0.1s;
    }

    .layer {
      position: absolute;
      top: 50%; left: 50%;
      transform: translate(-50%, -50%);
      border-radius: 20px;
      box-shadow: 0 0 40px rgba(255,255,255,0.6);
    }

    /* لایه پس‌زمینه نور */
    .layer.bg {
      width: 400px; height: 400px;
      background: radial-gradient(circle, rgba(255,255,255,0.15), transparent 70%);
      filter: blur(60px);
      z-index: -2;
    }

    /* لایه تصویر توکن */
    .layer.token {
      width: 300px;
      z-index: 1;
      animation: float 6s ease-in-out infinite;
    }

    @keyframes float {
      0%   { transform: translate(-50%, -50%) translateY(0px); }
      25%  { transform: translate(-50%, -50%) translateY(-20px); }
      50%  { transform: translate(-50%, -50%) translateY(0px); }
      75%  { transform: translate(-50%, -50%) translateY(20px); }
      100% { transform: translate(-50%, -50%) translateY(0px); }
    }

    /* دکمه شروع */
    .start-btn {
      position: relative;
      margin-top: 350px;
      padding: 15px 30px;
      font-size: 20px;
      border: none;
      border-radius: 15px;
      background: linear-gradient(90deg, #ff4d4d, #ff9933);
      color: white;
      cursor: pointer;
      box-shadow: 0 0 20px rgba(255,153,51,0.6);
      transition: transform 0.3s, box-shadow 0.3s;
      z-index: 2;
    }

    .start-btn:hover {
      transform: scale(1.1);
      box-shadow: 0 0 40px rgba(255,153,51,0.8);
    }
  </style>
</head>
<body>
  <div class="hero" id="hero">
    <div class="layer bg"></div>
    <img src="ai-token.png" alt="توکن AI" class="layer token">
    <button class="start-btn" onclick="startAction()">شروع کنید</button>
  </div>

  <script>
    const hero = document.getElementById('hero');

    // افکت حرکت موس برای حس 3D
    document.addEventListener('mousemove', (e) => {
      const x = (window.innerWidth / 2 - e.pageX) / 20;
      const y = (window.innerHeight / 2 - e.pageY) / 20;
      hero.style.transform = `rotateY(${x}deg) rotateX(${y}deg)`;
    });

    function startAction() {
      alert("کاربر روی شروع کلیک کرد! اینجا می‌توانید فرم یا اتصال به سرور قرار دهید.");
    }
  </script>
</body>
</html>
