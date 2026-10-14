

<html lang="ru">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#080808">
<title>Нурбек | 38 лет</title>

<style>
:root {
  --gold: #d8b66a;
  --black: #080808;
  --muted: #b8b2a5;
}
* { box-sizing: border-box; }
html { scroll-behavior: smooth; }

.header-photo {
  width: 220px;
  height: 220px;
  object-fit: cover;
  border-radius: 8px;
  border: 2px solid #d8b66a;
  padding: 4px;
  margin-bottom: 24px;
  box-shadow: 0 0 25px #d8b66a44;
  position: relative;
  z-index: 1;
}
body {
  margin: 0;
  color: #fff;
  background: var(--black);
  font-family: Georgia, "Times New Roman", serif;
  text-align: center;
}
.hero {
  min-height: 100svh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding: 55px 22px;
  position: relative;
  overflow: hidden;
  background:
    radial-gradient(ellipse at 50% 42%,
      #49371a 0%, #21180c 24%,
      #0c0b09 58%, #050505 100%);
}
.hero::before {
  content: "";
  position: absolute;
  inset: 18px;
  border: 1px solid #c9a85b66;
  pointer-events: none;
}
.eyebrow {
  color: var(--gold);
  letter-spacing: 5px;
  font: 11px Arial, sans-serif;
  text-transform: uppercase;
}
h1 {
  font-size: clamp(65px, 16vw, 125px);
  font-weight: 400;
  letter-spacing: 4px;
  margin: 20px 0 0;
  color: var(--gold);
  text-shadow: 0 0 35px #d8b66a22;
}
.age {
  font-size: clamp(20px, 5vw, 32px);
  letter-spacing: 8px;
  margin-top: 8px;
}
.line {
  width: 100px;
  height: 1px;
  background: var(--gold);
  margin: 28px auto;
}
.intro {
  max-width: 440px;
  color: #e3dccd;
  line-height: 1.8;
  font-size: 17px;
}
button, .btn {
  display: inline-block;
  border: 1px solid var(--gold);
  padding: 15px 24px;
  color: var(--gold);
  background: transparent;
  text-decoration: none;
  font: 12px Arial, sans-serif;
  letter-spacing: 2px;
  text-transform: uppercase;
  cursor: pointer;
  transition: .25s;
}
button:hover, .btn:hover {
  background: var(--gold);
  color: #080808;
}
.gold-button {
  color: #080808;
  background: var(--gold);
}
section {
  padding: 75px 22px;
  max-width: 760px;
  margin: auto;
}
h2 {
  color: var(--gold);
  font-size: 30px;
  font-weight: 400;
  margin: 0 0 20px;
}
p { line-height: 1.8; }
.muted { color: var(--muted); }
.countdown {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 10px;
  max-width: 500px;
  margin: 35px auto;
}
.time {
  padding: 17px 4px;
  border: 1px solid #b8974d55;
}
.time strong {
  display: block;
  font-size: clamp(25px, 6vw, 38px);
  font-weight: 400;
  color: var(--gold);
}
.time span {
  display: block;
  font: 10px Arial, sans-serif;
  color: var(--muted);
  margin-top: 10px;
  text-transform: uppercase;
}
.details {
  border-top: 1px solid #b8974d55;
  border-bottom: 1px solid #b8974d55;
  padding: 25px 10px;
  margin: 25px 0;
}
.detail {
  margin: 22px 0;
}
.detail b {
  display: block;
  color: var(--gold);
  font-weight: 400;
  margin-bottom: 8px;
  letter-spacing: 2px;
}
.actions {
  display: flex;
  gap: 12px;
  justify-content: center;
  flex-wrap: wrap;
  margin-top: 28px;
}
footer {
  color: #817969;
  padding: 30px 15px 45px;
  font: 11px Arial, sans-serif;
  letter-spacing: 3px;
}
.music {
  position: fixed;
  z-index: 5;
  right: 18px;
  bottom: 18px;
  width: 48px;
  height: 48px;
  border-radius: 50%;
  padding: 0;
  background: #15120b;
  box-shadow: 0 0 20px #000;
  letter-spacing: 0;
}
.music.playing { animation: pulse 2s infinite; }
@keyframes pulse {
  50% { box-shadow: 0 0 22px #d8b66a88; }
}
.reveal {
  opacity: 0;
  transform: translateY(20px);
  transition: opacity .8s, transform .8s;
}
.reveal.visible {
  opacity: 1;
  transform: translateY(0);
}
@media (prefers-reduced-motion: reduce) {
  *, *::before, *::after {
    scroll-behavior: auto !important;
    animation: none !important;
    transition: none !important;
  }
  .reveal { opacity: 1; transform: none; }
}
</style>
</head>

<body>

<header class="hero">
   <img src="nurbek.jpeg" alt="Нурбек" class="header-photo">
  
  <div class="eyebrow">A special evening</div>
  <h1>Нурбек</h1>
  <div class="age">38 ЛЕТ</div>
  <div class="line"></div>
  <p class="intro">
    Один особенный вечер.<br>
    Близкие люди, приятная атмосфера<br>
    и повод собраться вместе.
  </p>
  <p class="muted">Буду рад разделить этот день с тобой</p>
  <a class="btn gold-button" href="#invitation">
    Открыть приглашение
  </a>
</header>

<section id="invitation" class="reveal">
  <div class="eyebrow">You are invited</div>
  <div class="line"></div>
  <h2>Приглашаю тебя</h2>
  <p>
    На празднование моего 38-летия.<br>
    Будет здорово провести этот вечер вместе!
  </p>

  <h2 style="margin-top:45px">До встречи осталось</h2>
  <div class="countdown">
    <div class="time"><strong id="days">00</strong><span>Дней</span></div>
    <div class="time"><strong id="hours">00</strong><span>Часов</span></div>
    <div class="time"><strong id="minutes">00</strong><span>Минут</span></div>
    <div class="time"><strong id="seconds">00</strong><span>Секунд</span></div>
  </div>
  <p id="timerMessage" class="muted"></p>
</section>

<section class="reveal">
  <div class="eyebrow">Event details</div>
  <div class="line"></div>
  <h2>Детали вечера</h2>

  <div class="details">
    <div class="detail">
      <b>ДАТА</b>
      <span id="dateText">Укажите дату праздника</span>
    </div>
    <div class="detail">
      <b>ВРЕМЯ</b>
      <span id="timeText">Укажите время</span>
    </div>
    <div class="detail">
      <b>АДРЕС</b>
      <span id="venueText">Укажите название заведения</span>
    </div>
    <div class="detail">
      <b>МЕСТО</b>
      <span id="addressText">Укажите адрес мероприятия</span>
    </div>
  </div>

  <div class="actions">
    <a class="btn" id="mapButton" href="#"
       target="_blank" rel="noopener">
      Открыть карту
    </a>
    <a class="btn gold-button" id="rsvpButton" href="#">
      Подтвердить участие
    </a>
  </div>
  <p class="muted" style="font-size:13px">
    Пожалуйста, сообщи, сможешь ли прийти.
  </p>
</section>

<section class="reveal">
  <div class="line"></div>
  <h2>До скорой встречи!</h2>
  <p class="muted">Нурбек · 38</p>
</section>

<footer>WITH PLEASURE · NURBEK · 38</footer>

<button class="music" id="musicButton">♫</button>
        

<audio id="music" src="music.mp3" loop preload="auto"></audio>

<script>
// ===== НАСТРОЙКИ: ИЗМЕНИ ЭТИ ДАННЫЕ =====
const EVENT = {
  // Формат: ГГГГ-ММ-ДДTЧЧ:ММ:СС+05:00
  date: "2026-11-07T18:00:00+05:00",
  dateText: "7 ноябрь 2026 года",
  timeText: "18:00",
  address: "Apple city",
  venue: "183 квартира",
  
  // Номер WhatsApp: только цифры, с кодом страны.
  // Пример формата для Казахстана: 87075080877
  whatsapp: "+7 707 508 0877",

  // Вставь ссылку на место в Google Maps.
  mapUrl: "https://maps.app.goo.gl/Me7t3Csmw84sbxYF7?g_st=aw"
};
// ========================================

document.getElementById("dateText").textContent = EVENT.dateText;
document.getElementById("timeText").textContent = EVENT.timeText;
document.getElementById("venueText").textContent = EVENT.venue;
document.getElementById("addressText").textContent = EVENT.address;
document.getElementById("mapButton").href = EVENT.mapUrl;

document.getElementById("rsvpButton").href =
  "https://wa.me/" + EVENT.whatsapp +
  "?text=" + encodeURIComponent(
    "Привет, Нурбек! Отвечаю на приглашение на твой день рождения. "
  );

const target = new Date(EVENT.date).getTime();

function updateCountdown() {
  const now = Date.now();
  const diff = target - now;
  const message = document.getElementById("timerMessage");

  if (Number.isNaN(target)) {
    message.textContent = "Проверь дату в настройках сайта.";
    return;
  }

  if (diff <= 0) {
    ["days", "hours", "minutes", "seconds"].forEach(id => {
      document.getElementById(id).textContent = "00";
    });
    message.textContent = "Сегодня особенный день!";
    return;
  }

  const values = {
    days: Math.floor(diff / 86400000),
    hours: Math.floor(diff / 3600000) % 24,
    minutes: Math.floor(diff / 60000) % 60,
    seconds: Math.floor(diff / 1000) % 60
  };

  Object.entries(values).forEach(([id, value]) => {
    document.getElementById(id).textContent =
      String(value).padStart(2, "0");
  });
}

updateCountdown();
setInterval(updateCountdown, 1000);

// Музыка включается только после нажатия пользователя.
const audio = document.getElementById("music");
const musicButton = document.getElementById("musicButton");

musicButton.addEventListener("click", async () => {
  if (audio.paused) {
    try {
      await audio.play();
      musicButton.textContent = "Ⅱ";
      musicButton.classList.add("playing");
    } catch {
      alert("Не удалось включить музыку. Проверь файл music.mp3.");
    }
  } else {
    audio.pause();
    musicButton.textContent = "♫";
    musicButton.classList.remove("playing");
  }
});

// Плавное появление секций.
const observer = new IntersectionObserver(entries => {
  entries.forEach(entry => {
    if (entry.isIntersecting) {
      entry.target.classList.add("visible");
      observer.unobserve(entry.target);
    }
  });
}, { threshold: 0.12 });

document.querySelectorAll(".reveal").forEach(section => {
  observer.observe(section);
});
</script>
</body>
</html>
