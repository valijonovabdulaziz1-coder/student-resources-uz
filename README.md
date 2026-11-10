
<!DOCTYPE html>
<html lang="uz">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Student Resources UZ</title>
<style>
*{box-sizing:border-box}
body{margin:0;font-family:Arial;background:#f1f5f9;color:#172554}
header{background:#172554;color:white;text-align:center;padding:45px 15px}
nav{background:#2448ad;padding:16px;text-align:center}
nav a{color:white;text-decoration:none;margin:12px}
.languages{padding:18px;text-align:center}
button{padding:10px 20px;margin:5px;border:0;border-radius:8px;cursor:pointer;background:#2448ad;color:white}
button:hover{background:#172554}
main{max-width:1000px;margin:30px auto;padding:15px}
.card{background:white;padding:25px;margin:18px 0;border-radius:15px;box-shadow:0 4px 14px #0001}
.card a{color:#2452bd;font-weight:bold}
footer{background:#172554;color:white;text-align:center;padding:25px}
</style>
</head>
<body>

<header>
<h1>🎓 Student Resources UZ</h1>
<p id="subtitle">O‘zbekiston talabalari uchun bepul ta'lim platformasi</p>
</header>

<nav>
<a href="#" id="home">Bosh sahifa</a>
<a href="#lessons" id="lessonsLink">Darslar</a>
<a href="#about" id="aboutLink">Biz haqimizda</a>
</nav>

<div class="languages">
<button onclick="changeLang('uz')">🇺🇿 O‘zbekcha</button>
<button onclick="changeLang('ru')">🇷🇺 Русский</button>
<button onclick="changeLang('en')">🇬🇧 English</button>
</div>

<main>
<div class="card">
<h2 id="welcome">Talabalar uchun foydali platforma</h2>
<p id="description">Bu yerda Word, Excel, iqtisodiyot va kompyuter bo‘yicha o‘quv materiallarini topishingiz mumkin.</p>
</div>

<h2 id="materials">📚 O‘quv materiallari</h2>

<div class="card">
<h3 id="wordTitle">📄 Microsoft Word</h3>
<p id="wordDesc">Word dasturini noldan o‘rganing.</p>
<a href="word/first-lesson.md" id="wordLink">Word darsini ochish</a>
</div>

<div class="card">
<h3 id="excelTitle">📊 Microsoft Excel</h3>
<p id="excelDesc">Excel dasturini noldan o‘rganing.</p>
<a href="excel/first-lesson.md" id="excelLink">Excel darsini ochish</a>
</div>

<div class="card">
<h3 id="economyTitle">💰 Iqtisodiyot</h3>
<p id="economyDesc">Iqtisodiyot fanidan o‘quv materiallari.</p>
</div>

<div class="card">
<h3 id="computerTitle">💻 Kompyuter savodxonligi</h3>
<p id="computerDesc">Kompyuter va texnologiyalarni o‘rganing.</p>
</div>

<div class="card" id="about">
<h2 id="aboutTitle">Biz haqimizda</h2>
<p id="aboutDesc">Biz talabalar uchun bepul bilim va ta'lim resurslarini taqdim etamiz.</p>
</div>
</main>

<footer>
<p>© 2026 Student Resources UZ</p>
<p id="footerText">Barcha huquqlar himoyalangan.</p>
</footer>

<script>
const translations = {
uz: {
subtitle:"O‘zbekiston talabalari uchun bepul ta'lim platformasi",
home:"Bosh sahifa",lessonsLink:"Darslar",aboutLink:"Biz haqimizda",
welcome:"Talabalar uchun foydali platforma",
description:"Bu yerda Word, Excel, iqtisodiyot va kompyuter bo‘yicha o‘quv materiallarini topishingiz mumkin.",
materials:"📚 O‘quv materiallari",
wordTitle:"📄 Microsoft Word",wordDesc:"Word dasturini noldan o‘rganing.",wordLink:"Word darsini ochish",
excelTitle:"📊 Microsoft Excel",excelDesc:"Excel dasturini noldan o‘rganing.",excelLink:"Excel darsini ochish",
economyTitle:"💰 Iqtisodiyot",economyDesc:"Iqtisodiyot fanidan o‘quv materiallari.",
computerTitle:"💻 Kompyuter savodxonligi",computerDesc:"Kompyuter va texnologiyalarni o‘rganing.",
aboutTitle:"Biz haqimizda",aboutDesc:"Biz talabalar uchun bepul bilim va ta'lim resurslarini taqdim etamiz.",
footerText:"Barcha huquqlar himoyalangan."
},
ru: {
subtitle:"Бесплатная образовательная платформа для студентов Узбекистана",
home:"Главная",lessonsLink:"Уроки",aboutLink:"О нас",
welcome:"Полезная платформа для студентов",
description:"Здесь вы найдёте учебные материалы по Word, Excel, экономике и компьютерам.",
materials:"📚 Учебные материалы",
wordTitle:"📄 Microsoft Word",wordDesc:"Изучайте Word с нуля.",wordLink:"Открыть урок Word",
excelTitle:"📊 Microsoft Excel",excelDesc:"Изучайте Excel с нуля.",excelLink:"Открыть урок Excel",
economyTitle:"💰 Экономика",economyDesc:"Учебные материалы по экономике.",
computerTitle:"💻 Компьютерная грамотность",computerDesc:"Изучайте компьютеры и технологии.",
aboutTitle:"О нас",aboutDesc:"Мы предоставляем бесплатные образовательные ресурсы для студентов.",
footerText:"Все права защищены."
},
en: {
subtitle:"Free educational platform for students in Uzbekistan",
home:"Home",lessonsLink:"Lessons",aboutLink:"About us",
welcome:"A useful platform for students",
description:"Find learning materials about Word, Excel, economics and computers here.",
materials:"📚 Learning materials",
wordTitle:"📄 Microsoft Word",wordDesc:"Learn Word from scratch.",wordLink:"Open Word lesson",
excelTitle:"📊 Microsoft Excel",excelDesc:"Learn Excel from scratch.",excelLink:"Open Excel lesson",
economyTitle:"💰 Economics",economyDesc:"Educational materials about economics.",
computerTitle:"💻 Computer literacy",computerDesc:"Learn computers and technology.",
aboutTitle:"About us",aboutDesc:"We provide free educational resources for students.",
footerText:"All rights reserved."
}
};

function changeLang(lang) {
const t=translations[lang];
for (const id in t) {
document.getElementById(id).textContent=t[id];
}
document.documentElement.lang=lang;
}
</script>
</body>
</html>
