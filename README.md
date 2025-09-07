
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Happy Birthday 🎉</title>
  <style>
    body {
      margin: 0;
      height: 100vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      background: linear-gradient(to bottom, #fbcfe8, #fef3c7);
      font-family: Arial, sans-serif;
    }
    .cake {
      position: relative;
      width: 200px;
      height: 200px;
    }
    .layer {
      position: absolute;
      bottom: 0;
      border-radius: 10px 10px 0 0;
      box-shadow: 0 4px 10px rgba(0,0,0,0.2);
      transform: scaleY(0);
      transform-origin: bottom;
      animation: grow 0.8s forwards;
    }
    .layer1 { width: 200px; height: 65px; background: #f472b6; animation-delay: 0s; }
    .layer2 { width: 160px; height: 50px; background: #fde047; left: 20px; bottom: 65px; animation-delay: 0.8s; }
    .layer3 { width: 120px; height: 40px; background: #fff; left: 40px; bottom: 115px; animation-delay: 1.6s; }
    .candle {
      position: absolute;
      width: 10px;
      height: 40px;
      background: #ca8a04;
      left: 95px;
      bottom: 155px;
      opacity: 0;
      animation: fadeIn 0.5s forwards 2.4s;
    }
    .flame {
      position: absolute;
      width: 20px;
      height: 20px;
      background: orange;
      border-radius: 50%;
      left: 90px;
      bottom: 190px;
      transform: scale(0);
      animation: pulse 0.6s infinite 2.6s;
    }
    @keyframes grow { to { transform: scaleY(1); } }
    @keyframes fadeIn { to { opacity: 1; } }
    @keyframes pulse { 0%,100% { transform: scale(1);} 50% { transform: scale(1.2);} }
    h1, h2 {
      text-align: center;
      margin: 10px 0;
      opacity: 0;
      transform: translateY(20px);
      animation: fadeUp 1s forwards;
    }
    h1 { color: #be185d; font-size: 2em; animation-delay: 3s; }
    h2 { color: #444; font-size: 1.2em; animation-delay: 3.5s; }
    @keyframes fadeUp { to { opacity: 1; transform: translateY(0); } }
  </style>
</head>
<body>
  <div class="cake">
    <div class="layer layer1"></div>
    <div class="layer layer2"></div>
    <div class="layer layer3"></div>
    <div class="candle"></div>
    <div class="flame"></div>
  </div>
  <h1>🎉 Happy Birthday 🎉</h1>
  <h2>Michael Oleveros Cabus</h2>
</body>
</html>
