<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Important Question 👀</title>
  <link href="https://fonts.googleapis.com/css2?family=Pacifico&family=Fredoka+One&display=swap" rel="stylesheet">
  <style>
    body {
      height: 100vh;
      margin: 0;
      display: flex;
      align-items: center;
      justify-content: center;
      background: linear-gradient(135deg, #ff9a9e, #fad0c4);
      font-family: 'Fredoka One', cursive;
      text-align: center;
      overflow: hidden;
    }

    .box {
      background: rgba(255, 255, 255, 0.95);
      padding: 40px;
      border-radius: 25px;
      box-shadow: 0 10px 30px rgba(0,0,0,0.2);
      max-width: 90%;
    }

    h1 {
      font-family: 'Pacifico', cursive;
      color: #ff4d6d;
      margin-bottom: 5px;
      font-size: 2.2em;
    }

    p {
      font-size: 16px;
      margin-bottom: 20px;
      color: #555;
    }

    h2 {
      font-size: 1.6em;
      margin-bottom: 25px;
      color: #ff1e56;
    }

    button {
      font-size: 18px;
      padding: 12px 30px;
      border-radius: 30px;
      border: none;
      cursor: pointer;
      margin: 10px;
      transition: transform 0.2s;
    }

    #yes {
      background: #ff4d6d;
      color: white;
    }

    #no {
      background: #ccc;
      position: fixed;
      bottom: 30px;
      right: 30px;
      z-index: 1000;
    }

    button:hover {
      transform: scale(1.1);
    }
  </style>
</head>
<body>

  <div class="box">
    <h1>Hema Narayana Prabhu Vijayakumar </h1>
    <p>(aka Prabhu, calm down)</p>
    <h2>Will you be my Valentine? 🥺</h2>
    <p>Think carefully. Very carefully.</p>
    <button id="yes" onclick="yesClicked()">YES 🥰</button>
  </div>

  <button id="no">NO 🙄</button>

  <script>
    const noBtn = document.getElementById("no");

    noBtn.addEventListener("mouseover", () => {
      const x = Math.random() * (window.innerWidth - 120);
      const y = Math.random() * (window.innerHeight - 120);
      // Keep it away from top 180px (where the main box is)
      noBtn.style.left = x + "px";
      noBtn.style.top = Math.max(y, 180) + "px";
    });

    function yesClicked() {
      document.body.innerHTML = `
        <div style="
          height:100vh;
          display:flex;
          align-items:center;
          justify-content:center;
          flex-direction:column;
          background:linear-gradient(135deg,#ff9a9e,#fad0c4);
          font-family:'Fredoka One', cursive;
          text-align:center;
          padding:20px;
        ">
          <h1 style="font-family:'Pacifico', cursive; color:#ff1e56;">GOOD BOY 😏</h1>
          <h2>Prabhu is officially my Valentine </h2>
          </p>
        </div>
      `;
    }
  </script>

</body>
</html>
