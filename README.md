<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>SKYLINE FAMILY</title>
  <style>
    body {
      font-family: 'Segoe UI', sans-serif;
      margin: 0;
      background: #8f9aa0;
      color: #000;
    }
    header {
      background: #8f9aa0;
      padding: 20px;
      text-align: center;
      font-size: 46px;
      font-weight: bold;
      letter-spacing: 2px;
      font-family: 'Courier New', Courier, monospace;
    }
    nav {
      display: flex;
      justify-content: center;
      gap: 30px;
      background: #8f9aa0;
      padding: 10px;
      font-size: 18px;
    }
    nav a {
      text-decoration: none;
      color: #000;
    }
    .main-image {
      position: relative;
      text-align: center;
      margin-top: 20px;
    }
    .main-image img {
      width: 80%;
      max-width: 800px;
      border-radius: 10px;
    }
    .main-image .circle {
      position: absolute;
      top: 20px;
      right: 20px;
      background: #000;
      color: #8f9aa0;
      border-radius: 50%;
      padding: 10px 15px;
      font-weight: bold;
    }
    .content {
      display: flex;
      justify-content: space-around;
      margin: 40px 20px;
    }
    .column {
      width: 30%;
    }
    .column h3 {
      margin-bottom: 10px;
    }
    .chat-selector {
      display: flex;
      flex-direction: column;
      gap: 10px;
    }
    .chat-window {
      display: none;
      margin-top: 20px;
      padding: 10px;
      background: #55788a;
      border: 1px solid #ccc;
      border-radius: 5px;
    }
    footer {
      text-align: center;
      padding: 20px;
      background: #55788a;
      font-size: 14px;
    }
  </style>
  <script>
    function showChat(chatId) {
      const chats = document.querySelectorAll('.chat-window');
      chats.forEach(chat => chat.style.display = 'none');
      document.getElementById(chatId).style.display = 'block';
    }
  </script>
</head>
<body>

  <header>SKYLINE FAMILY</header>

  <nav>
    <a href="#">Our team</a>
    <a href="#">Administration</a>
    <a href="#">Music<a>
</nav>

  <div class="main-image">
    <img src="c:\Users\E\Downloads\photo_2025-05-23_22-46-47.jpg" alt="Main Visual">
  </div>

  <div class="content">
    <div class="column">
      <h3>Chat Selector</h3>
      <div class="chat-selector">
        <button onclick="showChat('chat1')">CHAT 1</button>
        <button onclick="showChat('chat2')">CHAT 2</button>
        <button onclick="showChat('chat3')">CHAT 3</button>
             
        </body>
      </div>

      <div id="chat1" class="chat-window">
        <h4>CHAT 1: Cozy Vibes</h4>
        <p>Добро пожаловать в уютный чат. Здесь царит спокойствие и ламповая атмосфера.</p>
        <audio controls>
          <source src="c:\Users\E\Downloads\Forg Chat 1.mp3" type="audio/mpeg">
        </audio>
      </div>

      <div id="chat2" class="chat-window">
        <h4>CHAT 2: Urban Pulse</h4>
        <p>Городская эстетика, ритмы мегаполиса и динамичные разговоры.</p>
        <audio controls>
          <source src="c:\Users\E\Downloads\Away Chat 2.m4a" type="audio/mpeg">
        </audio>
      </div>

      <div id="chat3" class="chat-window">
        <h4>CHAT 3: Dreamspace</h4>
        <p>Место для мечтателей, вдохновения и креативных идей.</p>
        <audio controls>
          <source src="c:\Users\E\Downloads\First Chat 3.mp3" type="audio/mpeg">
        </audio>
      </div>
    </div>

    <div class="column">
      <h3>Opening Date</h3>
      <p><strong>12 November 2023</strong><br>
      Our new website is finally live! Explore the new features and design.</p>
    </div>

    <div class="column">
      <h3>Dream Team Project</h3>
      <ul>
        <li>Vibe</li>
        <li>Teamwork</li>
        <li>Illustration</li>
      </ul>
    </div>
  </div>

  <footer>
    SKYLINE FAMILY © 2025 | Privacy Policy
  </footer>

</body>
</html>
<div style="text-align: center; margin: 20px;">
  <a href="https://t.me/SkylineProject" target="_blank" style="
    display: inline-block;
    background-color: #8f9aa0;
    color: white;
    padding: 12px 24px;
    font-size: 16px;
    border-radius: 6px;
    text-decoration: none;
    font-weight: bold;
    box-shadow: 0 4px 6px rgba(0,0,0,0.1);
    transition: background-color 0.3s ease;
  " onmouseover="this.style.backgroundColor='#8f9aa0'" onmouseout="this.style.backgroundColor='#314047'">
      Перейти в Telegram-канал c вашим вайбом 🚀
  </a>
</div>

<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <title>Информационная кнопка</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      padding: 40px;
      background-color: #55788a;
    }

    .info-button {
      background-color: #55788a;
      color: white;
      padding: 12px 24px;
      border: none;
      border-radius: 6px;
      font-size: 16px;
      cursor: pointer;
      font-weight: bold;
      box-shadow: 0 4px 6px rgba(0,0,0,0.1);
      transition: background-color 0.3s ease;
    }

    .info-button:hover {
      background-color: #426475;
    }

    .popup {
      display: none;
      position: fixed;
      top: 30%;
      left: 50%;
      transform: translate(-50%, -30%);
      background-color: #55788a;
      padding: 20px;
      border: 2px solid   #2f4550;
      border-radius: 10px;
      box-shadow: 0 8px 16px rgba(0,0,0,0.2);
      z-index: 1000;
      width: 300px;
      text-align: center;
    }

    .popup h3 {
      margin-top: 0;
    }

    .close-btn {
      margin-top: 15px;
      background-color: #8f9aa0;
      border: none;
      padding: 8px 16px;
      border-radius: 4px;
      cursor: pointer;
    }

    .overlay {
      display: none;
      position: fixed;
      top: 0; left: 0;
      width: 100%; height: 100%;
      background: rgba(0,0,0,0.4);
      z-index: 999;
    }
  </style>
</head>
<body>


  <button class="info-button" onclick="openPopup()">Подробнее о нас</button>

  <div class="overlay" id="overlay"></div>

  <div class="popup" id="popup">
    <h3>Информация о проекте</h3>
    <p>Добро пожаловать в DREAM TEAM PROJECT! Это творческий проект, где мы делимся эстетикой наших чатов, музыкой и вдохновением.</p>
    <button class="close-btn" onclick="closePopup()">Закрыть</button>
  </div>

  <script>
    function openPopup() {
      document.getElementById('popup').style.display = 'block';
      document.getElementById('overlay').style.display = 'block';
    }

    function closePopup() {
      document.getElementById('popup').style.display = 'none';
      document.getElementById('overlay').style.display = 'none';
    }
  </script>

</body>
</html>

<div class="column">
  <h3>MEM ZONE</h3>

  <!-- Мемы по умолчанию -->
  <div id="memeGallery" style="text-align:center;">
    <div class="meme">
      <img src="c:\Users\E\Downloads\koecu.jpg" alt="Meme 1" style="width:100%; max-width:250px; border-radius:10px;">
      <p>Когда подумал о своей жизни</p>
    </div>
  </div>

  <!-- Форма добавления -->
  <div style="margin-top:20px;">
    <h4>Добавь свой мем</h4>
    <input type="text" id="memeUrl" placeholder="Ссылка на изображение" style="width:100%; padding:8px; margin-bottom:10px;">
    <input type="text" id="memeText" placeholder="Подпись к мему" style="width:100%; padding:8px; margin-bottom:10px;">
    <button onclick="addMeme()" style="padding:10px 20px; background:#314047; color:white; border:none; border-radius:6px; cursor:pointer;">Добавить</button>
  </div>
</div>

<script>
  function addMeme() {
    const url = document.getElementById("memeUrl").value;
    const text = document.getElementById("memeText").value;

    if (url.trim() === "" || text.trim() === "") {
      alert("Пожалуйста, заполни оба поля.");
      return;
    }

    const memeDiv = document.createElement("div");
    memeDiv.className = "meme";
    memeDiv.innerHTML = `
      <img src="${url}" alt="User Meme" style="width:100%; max-width:250px; border-radius:10px; margin-top:15px;">
      <p>${text}</p>
    `;

    document.getElementById("memeGallery").appendChild(memeDiv);

    // Очистить поля
    document.getElementById("memeUrl").value = "";
    document.getElementById("memeText").value = "";
  }
</script>

<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <title>Mood Generator</title>
  <style>
    body {
      font-family: 'Segoe UI', sans-serif;
      margin: 0;
      padding: 0;
      text-align: center;
      transition: background 1s ease;
    }

    .mood-container {
      padding: 60px 20px;
    }

    .mood-btn {
      background-color: #6a00ff;
      color: white;
      padding: 14px 28px;
      font-size: 18px;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      font-weight: bold;
      box-shadow: 0 6px 12px rgba(0,0,0,0.2);
      transition: background-color 0.3s ease;
    }

    .mood-btn:hover {
      background-color: #4b00b5;
    }

    .mood-visual {
      margin-top: 40px;
    }

    .mood-visual img {
      width: 80%;
      max-width: 500px;
      border-radius: 12px;
      box-shadow: 0 8px 16px rgba(0,0,0,0.2);
    }

    .mood-quote {
      margin-top: 20px;
      font-size: 22px;
      font-style: italic;
      color: #333;
    }

    audio {
      margin-top: 20px;
    }
  </style>
</head>
<body>
