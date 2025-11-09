<!-- index.html -->
<!DOCTYPE html>
<html lang="fa">
<head>
  <meta charset="UTF-8">
  <title>🎨 تولیدکننده رنگ تصادفی</title>
  <style>
    body {
      font-family: sans-serif;
      text-align: center;
      transition: background 0.5s;
      height: 100vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      background-color: #3498db;
      color: white;
    }
    #colorCode {
      font-size: 28px;
      margin: 20px 0;
      padding: 10px 20px;
      background: rgba(255,255,255,0.2);
      border-radius: 10px;
    }
    button {
      padding: 10px 20px;
      border: none;
      border-radius: 8px;
      background: #fff;
      color: #333;
      font-size: 16px;
      cursor: pointer;
      transition: 0.3s;
    }
    button:hover {
      background: #eee;
    }
  </style>
</head>
<body>
  <h1>🎨 تولیدکننده رنگ تصادفی</h1>
  <div id="colorCode">#3498db</div>
  <button onclick="generateColor()">🔄 رنگ جدید</button>

  <script>
    function generateColor() {
      const randomColor = '#' + Math.floor(Math.random() * 16777215).toString(16);
      document.body.style.backgroundColor = randomColor;
      document.getElementById("colorCode").textContent = randomColor;
      document.getElementById("colorCode").style.background = "rgba(255,255,255,0.2)";
    }
  </script>
</body>
</html>
