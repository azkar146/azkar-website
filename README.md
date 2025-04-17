let count = 0;

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
