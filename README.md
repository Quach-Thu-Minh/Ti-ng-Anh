<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Hobby Vocabulary Game</title>
  <style>
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background-color: #fdf6e3;
      color: #333;
      text-align: center;
      padding: 30px;
    }
    .card {
      background-color: #fff3cd;
      border: 2px solid #ffeeba;
      border-radius: 16px;
      padding: 20px;
      max-width: 500px;
      margin: 20px auto;
      box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
    }
    button {
      padding: 10px 20px;
      margin: 10px;
      border: none;
      border-radius: 10px;
      background-color: #ff6f61;
      color: white;
      font-weight: bold;
      cursor: pointer;
    }
    button:hover {
      background-color: #ff3b2e;
    }
  </style>
</head>
<body>
  <h1>🎲 Hobby Vocabulary Game 🎲</h1>
  <div class="card">
    <h2 id="hint">Click the button to get your word!</h2>
    <p id="translation"></p>
    <button onclick="generateWord()">🎉 Get Word 🎉</button>
  </div>

  <script>
    const vocabList = [
      { word: \"belong to\", meaning: \"thuộc về\" },
      { word: \"benefit\", meaning: \"lợi ích\" },
      { word: \"bug\", meaning: \"con bọ\" },
      { word: \"cardboard\", meaning: \"bìa cứng\" },
      { word: \"dollhouse\", meaning: \"nhà búp bê\" },
      { word: \"gardening\", meaning: \"làm vườn\" },
      { word: \"glue\", meaning: \"keo dán / hồ\" },
      { word: \"horse riding\", meaning: \"cưỡi ngựa\" },
      { word: \"insect\", meaning: \"côn trùng\" },
      { word: \"jogging\", meaning: \"đi/chạy bộ thư giãn\" },
      { word: \"making models\", meaning: \"làm mô hình\" },
      { word: \"maturity\", meaning: \"sự trưởng thành\" },
      { word: \"patient\", meaning: \"kiên nhẫn\" },
      { word: \"popular\", meaning: \"được yêu thích\" },
      { word: \"responsibility\", meaning: \"sự trách nhiệm\" },
      { word: \"set\", meaning: \"(mặt trời) lặn\" },
      { word: \"stress\", meaning: \"sự căng thẳng\" },
      { word: \"take on\", meaning: \"nhận thêm\" },
      { word: \"unusual\", meaning: \"khác thường\" },
      { word: \"valuable\", meaning: \"quý giá\" },
      { word: \"yoga\", meaning: \"yoga\" }
    ];

    function generateWord() {
      const index = Math.floor(Math.random() * vocabList.length);
      const vocab = vocabList[index];
      document.getElementById('hint').innerText = `Your word: ${vocab.word}`;
      document.getElementById('translation').innerText = `Meaning: ${vocab.meaning}`;
    }
  </script>
</body>
</html>

