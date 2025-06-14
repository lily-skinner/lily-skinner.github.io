<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Bubble Animation</title>
  <style>
    /* Page reset and dark background */
    body {
      margin: 0;
      padding: 0;
      background: #000;
      color: white;
      font-family: 'Segoe UI', sans-serif;
      overflow: hidden;
    }

    .content {
      position: relative;
      z-index: 2;
      padding: 100px 20px;
      text-align: center;
    }

    .content h1 {
      font-size: 3em;
      margin-bottom: 0.5em;
    }

    .content p {
      font-size: 1.5em;
    }

    /* Bubble container */
    .bubbles {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      overflow: hidden;
      z-index: 1;
    }

    .bubbles span {
      position: absolute;
      display: block;
      width: 40px;
      height: 40px;
      background: rgba(0, 150, 255, 0.2);
      border-radius: 50%;
      animation: rise 15s linear infinite;
      bottom: -100px;
    }

    .bubbles span:nth-child(odd) {
      background: rgba(0, 150, 255, 0.4);
    }

    /* Randomized animation for bubbles */
    @keyframes rise {
      0% {
        transform: translateY(0) scale(1);
        opacity: 1;
      }
      100% {
        transform: translateY(-1000px) scale(1.5);
        opacity: 0;
      }
    }

    /* Random positioning */
    .bubbles span {
      left: calc(100% * var(--i));
      animation-duration: calc(5s + 10s * var(--i));
      width: calc(20px + 20px * var(--i));
      height: calc(20px + 20px * var(--i));
    }
  </style>
</head>
<body>
  <div class="bubbles">
    <!-- Generate 20 bubbles with custom CSS variable for randomness -->
    <!-- You can use a script or manually write these -->
    <span style="--i: 0.05"></span>
    <span style="--i: 0.1"></span>
    <span style="--i: 0.15"></span>
    <span style="--i: 0.2"></span>
    <span style="--i: 0.25"></span>
    <span style="--i: 0.3"></span>
    <span style="--i: 0.35"></span>
    <span style="--i: 0.4"></span>
    <span style="--i: 0.45"></span>
    <span style="--i: 0.5"></span>
    <span style="--i: 0.55"></span>
    <span style="--i: 0.6"></span>
    <span style="--i: 0.65"></span>
    <span style="--i: 0.7"></span>
    <span style="--i: 0.75"></span>
    <span style="--i: 0.8"></span>
    <span style="--i: 0.85"></span>
    <span style="--i: 0.9"></span>
    <span style="--i: 0.95"></span>
  </div>

  <div class="content">
    <h1>Welcome to My Bubble Site</h1>
    <p>Text floats beautifully above animated bubbles 🌊</p>
  </div>
</body>
</html>
