body {
  font-family: 'Arial', sans-serif;
  background-color: #f9f9f9;
  margin: 0;
  padding: 0;
  text-align: center;
  direction: rtl;
}

.container {
  max-width: 600px;
  margin: auto;
  padding: 20px;
}

h1 {
  color: #2c3e50;
}

.zekr {
  background-color: #fff;
  padding: 20px;
  margin-top: 20px;
  border-radius: 12px;
  box-shadow: 0 0 10px #ddd;
}

.buttons {
  margin-top: 15px;
}

button {
  padding: 10px 15px;
  margin: 0 5px;
  border: none;
  border-radius: 8px;
  background-color: #3498db;
  color: white;
  cursor: pointer;
  font-size: 16px;
}

button:hover {
  background-color: #2980b9;
}

.links {
  list-style: none;
  padding: 0;
}

.links li {
  margin: 10px 0;
}

.links a {
  text-decoration: none;
  color: #3498db;
  font-size: 20px;
}<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8">
  <title>موقع الأذكار</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <div class="container">
    <h1>مرحباً بك في موقع الأذكار</h1>
    <ul class="links">
      <li><a href="azkar-sabah.html">أذكار الصباح</a></li>
      <li><a href="azkar-masaa.html">أذكار المساء</a></li>
      <li><a href="azkar-nawm.html">أذكار النوم</a></li>
    </ul>
  </div>
</body>
</html>let count = 0;

function copyZekr() {
  const text = document.getElementById("zekrText").innerText;
  navigator.clipboard.writeText(text).then(() => {
    alert("تم نسخ الذكر!");
  });
}

function incrementCount() {
  count++;
  document.getElementById("count").innerText = count;
}
<script src="script.js"></script>
<p id="zekrText">نص الذكر هنا</p>

<div class="buttons">
  <button onclick="copyZekr()">نسخ</button>
  <button onclick="incrementCount()">تكرار: <span id="count">0</span></button>
</div>
body {
  font-family: 'Arial', sans-serif;
  background-color: #f9f9f9;
  margin: 0;
  padding: 0;
  text-align: center;
  direction: rtl;
}

.container {
  max-width: 600px;
  margin: auto;
  padding: 20px;
}

h1 {
  color: #2c3e50;
}

.zekr {
  background-color: #fff;
  padding: 20px;
  margin-top: 20px;
  border-radius: 12px;
  box-shadow: 0 0 10px #ddd;
}

.buttons {
  margin-top: 15px;
}

button {
  padding: 10px 15px;
  margin: 0 5px;
  border: none;
  border-radius: 8px;
  background-color: #3498db;
  color: white;
  cursor: pointer;
  font-size: 16px;
}

button:hover {
  background-color: #2980b9;
}
