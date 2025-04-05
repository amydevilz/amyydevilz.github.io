# amydevilz.github.io
<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <title>happy bday</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      overflow: hidden;
      background: #AEC6CF;
      font-family: 'Arial', sans-serif;
      text-align: center;
      color: #333;
    }

    h1 {
      margin-top: 80px;
      font-size: 50px;
      color: #d36da3;
    }

    .button {
      margin-top: 30px;
      padding: 15px 30px;
      font-size: 20px;
      border: none;
      border-radius: 10px;
      background-color: #f7a8c6;
      color: white;
      cursor: pointer;
      transition: background 0.3s ease;
    }

    .button:hover {
      background-color: #ec6fa7;
    }

    .surprise-box {
      display: none;
      margin: 40px auto 0;
      background: white;
      border-radius: 20px;
      padding: 30px;
      width: 300px;
      box-shadow: 0 10px 30px rgba(0,0,0,0.2);
      animation: popUp 0.5s ease-out;
    }

    @keyframes popUp {
      from {
        transform: scale(0.5);
        opacity: 0;
      }
      to {
        transform: scale(1);
        opacity: 1;
      }
    }

    /* Balões animados */
    .balloon {
      position: absolute;
      bottom: -100px;
      width: 40px;
      height: 60px;
      background-color: pink;
      border-radius: 50% 50% 45% 45%;
      animation: floatUp 8s infinite ease-in;
    }

    .balloon::after {
      content: '';
      position: absolute;
      bottom: -20px;
      left: 50%;
      width: 2px;
      height: 20px;
      background: gray;
      transform: translateX(-50%);
    }

    @keyframes floatUp {
      0% { transform: translateY(0) rotate(0deg); opacity: 0; }
      10% { opacity: 1; }
      100% { transform: translateY(-120vh) rotate(360deg); opacity: 0; }
    }

    /* Variações de cor e posição dos balões */
    .balloon:nth-child(1) {
      left: 10%;
      background-color: #ffb6c1;
      animation-delay: 0s;
    }

    .balloon:nth-child(2) {
      left: 30%;
      background-color: #ffc1cc;
      animation-delay: 2s;
    }

    .balloon:nth-child(3) {
      left: 50%;
      background-color: #ffccd5;
      animation-delay: 4s;
    }

    .balloon:nth-child(4) {
      left: 70%;
      background-color: #fdaecb;
      animation-delay: 1s;
    }

    .balloon:nth-child(5) {
      left: 90%;
      background-color: #f9b2d4;
      animation-delay: 3s;
    }
  </style>
</head>
<body>

  <h1>here's a surprise for u!</h1>
  <button class="button" onclick="showSurprise()">Click aqui</button>

  <div class="surprise-box" id="surpriseBox">
    <h3>happy birthday davezinhoww!</h3>
    <a href='https://postimg.cc/YvBnWPVN' target='_blank'><img src='https://i.postimg.cc/YvBnWPVN/images-2.jpg' border='0' alt='images-2'/></a>
  </div> 

  <!-- Balões -->
  <div class="balloon"></div>
  <div class="balloon"></div>
  <div class="balloon"></div>
  <div class="balloon"></div>
  <div class="balloon"></div>

  <script>
    function showSurprise() {
      document.getElementById('surpriseBox').style.display = 'block';
    }
  </script>

</body>
</html>
