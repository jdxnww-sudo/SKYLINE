<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>SKYLINE FAMILY</title>
  <style>
    /* ------------------- ОСНОВНЫЕ СТИЛИ ------------------- */
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
      font-size: 58px;
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
      width: 100%;
      max-width: 1000px;
      border-radius: 20px;
    }
    .main-image .circle {
      position: absolute;
      top: 30px;
      right: 30px;
      background: #000;
      color: #8f9aa0;
      border-radius: 50%;
      padding: 10px 15px;
      font-weight: bold;
    }
    .content {
      display: flex;
      flex-wrap: wrap; /* Позволяет колонкам переноситься */
      justify-content: space-around;
      margin: 40px 20px;
    }
    .column {
      width: 30%;
      min-width: 250px; /* Минимальная ширина для лучшего отображения */
      margin-bottom: 20px;
      padding: 15px;
      background: #d4d4d4; /* Легкий фон для колонок */
      border-radius: 8px;
    }
    .column h3 {
      margin-bottom: 10px;
      border-bottom: 2px solid #55788a;
      padding-bottom: 5px;
    }
    .chat-selector {
      display: flex;
      flex-direction: column;
      gap: 10px;
    }
    .chat-selector button {
      padding: 10px;
      background-color: #55788a;
      color: white;
      border: none;
      border-radius: 6px;
      cursor: pointer;
      font-weight: bold;
    }
    .chat-selector button:hover {
      background-color: #314047;
    }
    .chat-window {
      display: none;
      margin-top: 20px;
      padding: 10px;
      background: #55788a;
      color: white;
      border: 1px solid #ccc;
      border-radius: 5px;
    }
    /footer {
      text-align: center;
      padding: 20px;
      background: #55788a;
      font-size: 14px;
      color: white;
      margin-top: 20px;
    }
    */
.
    .site-footer {
      width: 100%;
      background-color: #2c3e50; /* Темный, глубокий синий/серый цвет */
      color: #ecf0f1; /* Светлый, почти белый текст */
      padding: 15px 0; /* Внутренние отступы сверху и снизу */
      text-align: center; /* Центрирование текста */
      font-family: Arial, sans-serif; /* Хорошо читаемый шрифт */
      box-shadow: 0 -2px 5px rgba(0, 0, 0, 0.1); /* Легкая тень сверху */
      margin-top: 20px;
    }
    .footer-content p {
      margin: 0;
      font-size: 14px;
      letter-spacing: 0.5px;
      opacity: 0.9;
      margin-bottom: 10px; /* Отступ снизу от текста до кнопок */
    }
    /* Стиль для имени "So Vein" */
    .footer-content p span {
      font-weight: bold;
      color: #3498db; /* Акцентный синий цвет */
    }
    /* Стили для КНОПОК в футере */
    .footer-links {
      margin-top: 10px;
    }
    .footer-btn {
      display: inline-block;
      padding: 6px 15px;
      margin: 0 5px;
      background-color: #3498db;
      color: #ffffff;
      text-decoration: none;
      border-radius: 4px;
      font-size: 13px;
      transition: background-color 0.3s ease;
      border: none;
      cursor: pointer;
    }
    .footer-btn:hover {
      background-color: #2980b9; /* Чуть темнее при наведении */
    }
    /* ------------------- КОНЕЦ НОВЫХ СТИЛЕЙ ДЛЯ ФУТЕРА ------------------- */
    
    /* ------------------- СТИЛИ POP-UP (ИНФО) ------------------- */
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
      display: block; /* Занимает всю ширину колонки */
      width: 100%;
      box-sizing: border-box;
      margin-top: 10px;
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
      color: white;
      padding: 20px;
      border: 2px solid #2f4550;
      border-radius: 10px;
      box-shadow: 0 8p x 16px rgba(0,0,0,0.5);
      z-index: 1000;
      width: 300px;
      text-align: center;
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
      background: rgba(0,0,0,0.6);
      z-index: 999;
    }
    /* ------------------- СТИЛИ TELEGRAM ------------------- */
    .telegram-link {
      text-align: center;
      margin: 20px 0;
    }
    .telegram-link a {
      display: inline-block;
      background-color: #55788a;
      color: white;
      padding: 12px 24px;
      font-size: 16px;
      border-radius: 6px;
      text-decoration: none;
      font-weight: bold;
      box-shadow: 0 4px 6px rgba(0,0,0,0.1);
      transition: background-color 0.3s ease;
    }
    .telegram-link a:hover {
      background-color: #8f9aa0 !important; /* !important, чтобы переопределить inline-стиль */
    }
    /* ------------------- СТИЛИ MOOD GENERATOR ------------------- */
    .mood-container {
      padding: 10px 0;
    }
    .mood-btn {
      background-color: #6a00ff;
      color: white;
      padding: 10px 20px;
      font-size: 16px;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      font-weight: bold;
      box-shadow: 0 4px 8px rgba(0,0,0,0.2);
      transition: background-color 0.3s ease;
      margin-bottom: 10px;
    }
    .mood-btn:hover {
      background-color: #4b00b5;
    }
    .mood-visual {
      margin-top: 10px;
    }
    .mood-visual img {
      width: 90%;
      max-width: 300px;
      border-radius: 12px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.2);
    }
    .mood-quote {
      margin-top: 15px;
      font-size: 18px;
      font-style: italic;
      color: #333;
    }
    /* ------------------- МЕДИА-ЗАПРОСЫ ------------------- */
    @media (max-width: 1024px) {
        .column {
            width: 45%; /* Две колонки на средней ширине */
        }
    }
    @media (max-width: 767px) {
      header {
        font-size: 30px;
        padding: 15px;
      }
      nav {
        flex-direction: column;
        gap: 10px;
        padding: 10px 0;
        text-align: center;
      }
      .main-image img {
        width: 95%;
      }
      .main-image .circle {
        right: 5%;
        top: 10px;
        transform: none;
        padding: 8px 12px;
        font-size: 12px;
      }
      .content {
        margin: 20px 10px;
      }
      .column {
        width: 95%; /* Одна колонка на мобильных */
        max-width: none;
        margin: 10px auto;
        padding: 15px;
      }
      .chat-selector button, .info-button, .telegram-link a {
        padding: 10px;
        font-size: 15px;
      }
      .popup {
        width: 90%;
        max-width: 350px;
      }
    }
  </style>
</head>

<body>
  <header>SKYLINE FAMILY</header>

  <nav>
    <a href="#">Our team</a>
    <a href="#">Administration</a>
    <a href="#">Music</a>
  </nav>

  <div class="main-image">
    <img src="photo_2025-05-23_22-46-47.jpg" alt="Skyline Family Main Image" />
    <div class="circle">NEW</div>
  </div>

  <div class="content">

  <div class="column">
      <h3>Chat Selector</h3>
      <div class="chat-selector">
        <button onclick="showChat('chat1')">CHAT 1</button>
        <button onclick="showChat('chat2')">CHAT 2</button>
        <button onclick="showChat('chat3')">CHAT 3</button>
      </div>       <div id="chat1" class="chat-window">
        <h4>CHAT 1: Cozy Vibes</h4>
        <p>Добро пожаловать в уютный чат. Здесь царит спокойствие и ламповая атмосфера.</p>
        <audio controls>
          <source src="Forg Chat 1.mp3" type="audio/mpeg">
        </audio>
      </div>
      <div id="chat2" class="chat-window">
        <h4>CHAT 2: Urban Pulse</h4>
        <p>Городская эстетика, ритмы мегаполиса и динамичные разговоры.</p>
        <audio controls>
          <source src="Away Chat 2.m4a" type="audio/mpeg">
        </audio>
      </div>
      <div id="chat3" class="chat-window">
        <h4>CHAT 3: Dreamspace</h4>
        <p>Место для мечтателей, вдохновения и креативных идей.</p>
        <audio controls>
          <source src="First Chat 3.mp3" type="audio/mpeg">
        </audio>
      </div>
    </div>

   <div class="column">
      <h3>Opening Date</h3>
      <p><strong>12 November 2023</strong><br>
      Our new website is finally live! Explore the new features and design.</p>

  <h3>Dream Team Project</h3>
      <ul>
        <li>Vibe</li>
        <li>Teamwork</li>
        <li>Illustration</li>
      </ul>

  <button class="info-button" onclick="openPopup()">Подробнее о нас</button>
    </div>

  <div class="column">
      <h3>MEM ZONE</h3>
      <div id="memeGallery" style="text-align:center;">
        <div class="meme">
          <img src="https://via.placeholder.com/250x150?text=Meme+Placeholder" alt="Meme 1" style="width:100%; max-width:250px; border-radius:10px;">
          <p>Когда подумал о своей жизни</p>
        </div>
      </div>
      <div style="margin-top:20px;">
        <h4>Добавь свой мем</h4>
        <input type="text" id="memeUrl" placeholder="Ссылка на изображение" style="width:100%; padding:8px; margin-bottom:10px; box-sizing: border-box;">
        <input type="text" id="memeText" placeholder="Подпись к мему" style="width:100%; padding:8px; margin-bottom:10px; box-sizing: border-box;">
        <button onclick="addMeme()" style="padding:10px 20px; background:#314047; color:white; border:none; border-radius:6px; cursor:pointer;">Добавить</button>
      </div>
    </div>

  <div class="column">
      <h3>Mood Generator</h3>
      <div class="mood-container">
        <button class="mood-btn" onclick="generateMood()">Сгенерировать Настроение</button>
        <div class="mood-visual" id="moodVisual">
          <img src="https://via.placeholder.com/400x200?text=Нажмите+кнопку" alt="Mood Image">
          <p class="mood-quote" id="moodQuote">Нажмите, чтобы увидеть ваше настроение!</p>
          <audio controls id="moodAudio" style="display:none;"></audio>
        </div>
      </div>
    </div>

  </div> <div class="telegram-link">
    <a href="https://t.me/SkylineProject" target="_blank" onmouseover="this.style.backgroundColor='#8f9aa0'" onmouseout="this.style.backgroundColor='#55788a'">
      Перейти в Telegram-канал c вашим вайбом 🚀
    </a>
  </div>
  
<footer class="site-footer">
    <div class="footer-content">
        <p>&copy; 2025 Owner - <span>So Vein</span></p>
        
        <div class="footer-links">
            <a href="#" class="footer-btn">Контакты</a>
            <a href="#" class="footer-btn">О нас</a>
            <a href="#" class="footer-btn">Политика</a>
            <a href="#" class="footer-btn">Карта сайта</a>
        </div>
    </div>
</footer>
  <div class="overlay" id="overlay"></div>
  <div class="popup" id="popup">
    <h3>Информация о проекте</h3>
    <p>Добро пожаловать в DREAM TEAM PROJECT! Это творческий проект, где мы делимся эстетикой наших чатов, музыкой и вдохновением.</p>
    <button class="close-btn" onclick="closePopup()">Закрыть</button>
  </div>


 <script>
    function showChat(chatId) {
      const chats = document.querySelectorAll('.chat-window');
      chats.forEach(chat => chat.style.display = 'none');
      document.getElementById(chatId).style.display = 'block';
    }

    // ------------------- POP-UP (ИНФО КНОПКА) -------------------
    function openPopup() {
      document.getElementById('popup').style.display = 'block';
      document.getElementById('overlay').style.display = 'block';
    }

    function closePopup() {
      document.getElementById('popup').style.display = 'none';
      document.getElementById('overlay').style.display = 'none';
    }

    // ------------------- MEM ZONE -------------------
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

    // ------------------- MOOD GENERATOR -------------------
    const moods = [
      { quote: "Спокойствие в душе. Наслаждайся тишиной.", image: "https://via.placeholder.com/400x200?text=Cozy+Mood", audio: "Forg Chat 1.mp3" },
      { quote: "Ритм города зовет. Время действовать!", image: "https://via.placeholder.com/400x200?text=Urban+Vibe", audio: "Away Chat 2.m4a" },
      { quote: "Мечты сбываются. Ищи вдохновение в деталях.", image: "https://via.placeholder.com/400x200?text=Dreamy+Aura", audio: "First Chat 3.mp3" },
      { quote: "Полный релакс. Никаких забот.", image: "https://via.placeholder.com/400x200?text=Chill+Zone", audio: "" },
      { quote: "Энергия бьет ключом. Готов к новым свершениям.", image: "https://via.placeholder.com/400x200?text=High+Energy", audio: "" }
    ];

    function generateMood() {
      const randomIndex = Math.floor(Math.random() * moods.length);
      const mood = moods[randomIndex];

      const visualDiv = document.getElementById('moodVisual');
      visualDiv.querySelector('img').src = mood.image;
      document.getElementById('moodQuote').textContent = mood.quote;

      const audioPlayer = document.getElementById('moodAudio');
      if (mood.audio) {
        audioPlayer.src = mood.audio;
        audioPlayer.style.display = 'block';
        audioPlayer.load(); // Перезагрузка аудио
      } else {
        audioPlayer.style.display = 'none';
        audioPlayer.pause();
        audioPlayer.src = '';
      }
    }
  </script>

</body>
</html>

   
