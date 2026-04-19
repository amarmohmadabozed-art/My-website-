<!DOCTYPE html>
<html>
<head><style>
  body {
    background-color: black; 
    /* لون خلفية رمادي فاتح */
    font-family: Arial, sans-serif;      
  }
.logo {
    color: blue;
    font-size: 20px;
}

.menu a {
    color: red;
    margin-left: 14px;
    text-decoration: none;
}

  h1 {
    color: yellow; /* العنوان باللون الأزرق */
    font-size: 50px;
    text-align: center; /* يوسط العنوان في الصفحة */
    margin: 50px 0; 
  }
  p {
    color: white; /* الفقرة باللون الأخضر */
    font-size: 25px; /* حجم الخط */
    text-align: center;
    margin: 20px 0;
  }
  
  button {
   background-color: blue;
   color:white;
   font-size: 20px;
   border-radius: 50px;
   padding: 10px 20px;
   margin: 20px;
   transition: 0.3s;
  }
  
  button:active {
    transform: scale(1.2);
  background-color:red ;
  }
  .Ammar1 {
    display: flex;
    justify-content: center; /* أفقي */
    align-items: center;     /* رأسي */
    height: 10vh;           /* ياخد طول الصفحة */
}
.navbar {
    background-color:gold;
    padding: 15px;
    justify-content: space-between;   
    display: flex;
}
.footer {
    text-align: center;
    padding: 20px;
    background-color: gold;
    margin-top: 120px;
    color: red;

}
.Ammar2 {
      display: flex;
    justify-content: center;
    gap: 20px;
    flex-wrap: wrap;
    margin: 20px;
}

.card {
  background-color: gold;
  padding: 20px;
  font-size: 30px;
  height: 250px;
  width: 250px; /* تحكم في العرض */
  border-radius: 20px;
  margin: 20px;

  display: flex;
  flex-direction: column;
  justify-content: center; /* توسيط رأسي */
  align-items: center;     /* توسيط أفقي */   
  transition:0.3s;
}
.card:active {
    transform: translateY(-10px);
transition: 0.3s;
}


.card button {
  background-color: black;
  color: white;
  border: none;
  padding: 10px 15px;
  margin-top: 20px;
  font-size: 15px;
  border-radius: 10px;
  cursor: pointer;
  transition: 0.3s;
}
.card button:hover {
  transform: scale(1.4);
  background-color:red ;
}
.ABCD {
      text-align: center;
}
</style>
  <meta charset="UTF-8">
  <title>Ammar Mohammed</title>
</head>
<body>
  <div class="navbar">
    <div class="logo">Ammar</div>
    <div class="menu">
        <a href="#">Home</a>
        <a href="#">About</a>
        <a href="#">Contact</a>
    </div>
    </div>
  <!-- هنا تكتب المحتوى بتاعك -->
  <h1>Ammar is hero</h1>
  <div class="Ammar1">
   <button id="button1"onclick="changeText()">اضغط  هنا</button>
   </div>
  <p id="text1">Welcome to My App My name is Ammar, I'm from Egypt🇪🇬</p>
  
  <div class="Ammar2">
    
    <div class="card">
    <span>Aمطور الموقع</span>
    <button onclick="msg1()">انقر هنا</button>
    </div>
    
        <div class="card">
      <span>A1مساعد مطور </span>
    <button onclick="msg1()">انقر هنا</button>
    </div>
      
  </div>
  <div class="ABCD">
<button onclick="like1()"class="text">like👍
</button>
<p id="likes">0</p>
</div>
  <div class="footer">
    ©Ammar Website 2026
  </div>
 
 <script>
function changeText() {
    document.getElementById("text1").textContent = "Ammar is a great Egyptian 🔥";
    document.getElementById("text1").style.color = "gold";
}
function msg1() {
    alert ("مرحبا بك في موقعي😎") 
}

let count = 0;
function like1() {
    count++;
    document.getElementById("likes").innerHTML = count;
}
</script>
</body>
</html>
