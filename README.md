
<!DOCTYPE html>
<html lang="uz">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Student Resources — Ta'lim platformasi</title>

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    background: #f1f5f9;
    color: #1e293b;
}

header {
    background: linear-gradient(135deg, #123c69, #2563eb);
    color: white;
    text-align: center;
    padding: 45px 20px;
}

header h1 {
    font-size: 32px;
    margin-bottom: 12px;
}

header p {
    font-size: 16px;
}

.languages {
    text-align: center;
    padding: 20px;
}

.languages button {
    padding: 10px 18px;
    margin: 5px;
    border: none;
    border-radius: 8px;
    background: #2563eb;
    color: white;
    cursor: pointer;
    font-size: 15px;
}

.languages button:hover {
    background: #123c69;
}

.container {
    max-width: 1100px;
    margin: auto;
    padding: 20px;
}

.section-title {
    text-align: center;
    margin: 20px 0 25px;
    font-size: 27px;
}

.courses {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
    gap: 22px;
}

.card {
    background: white;
    padding: 25px;
    border-radius: 14px;
    box-shadow: 0 4px 15px rgba(0,0,0,0.08);
}

.card h2 {
    margin-bottom: 12px;
    color: #1d4ed8;
}

.card p {
    line-height: 1.6;
    margin-bottom: 18px;
}

.card a {
    display: inline-block;
    background: #2563eb;
    color: white;
    text-decoration: none;
    padding: 11px 17px;
    border-radius: 8px;
    margin-top: 8px;
}

.card a:hover {
    background: #123c69;
}

.lesson-list {
    margin-top: 15px;
}

.lesson-list a {
    display: block;
    margin: 8px 0;
    font-size: 14px;
}

footer {
    margin-top: 45px;
    padding: 25px;
    text-align: center;
    background: #123c69;
    color: white;
}

@media(max-width: 600px) {
    header h1 {
        font-size: 25px;
    }
}
</style>
</head>

<body>

<header>
    <h1 id="siteTitle">Student Resources</h1>
    <p id="siteDescription">Talabalar uchun bepul ta'lim platformasi</p>
</header>

<div class="languages">
    <button onclick="changeLanguage('uz')">O'zbekcha</button>
    <button onclick="changeLanguage('ru')">Русский</button>
    <button onclick="changeLanguage('en')">English</button>
</div>

<main class="container">

    <h2 class="section-title" id="coursesTitle">O'quv kurslari</h2>

    <div class="courses">

        <div class="card">
            <h2 id="wordTitle">Microsoft Word</h2>
            <p id="wordDescription">
                Matnli hujjatlar yaratish, tahrirlash va bezashni o'rganing.
            </p>
            <a href="word/10-lessons.md" id="wordLink">
                10 ta darsni boshlash
            </a>
        </div>

        <div class="card">
            <h2 id="excelTitle">Microsoft Excel</h2>
            <p id="excelDescription">
                Elektron jadvallar, formulalar va diagrammalar bilan ishlashni o'rganing.
            </p>
            <a href="excel/10-lessons.md" id="excelLink">
                10 ta darsni boshlash
            </a>
        </div>

        <div class="card">
            <h2 id="economicsTitle">Iqtisodiyot</h2>
            <p id="economicsDescription">
                Iqtisodiyot fanining asosiy tushunchalari va mavzularini o'rganing.
            </p>

            <div class="lesson-list" id="economicsLessons">
                <a href="economics/10-lessons.md#lesson-1">1-dars</a>
                <a href="economics/10-lessons.md#lesson-2">2-dars</a>
                <a href="economics/10-lessons.md#lesson-3">3-dars</a>
                <a href="economics/10-lessons.md#lesson-4">4-dars</a>
                <a href="economics/10-lessons.md#lesson-5">5-dars</a>
                <a href="economics/10-lessons.md#lesson-6">6-dars</a>
                <a href="economics/10-lessons.md#lesson-7">7-dars</a>
                <a href="economics/10-lessons.md#lesson-8">8-dars</a>
                <a href="economics/10-lessons.md#lesson-9">9-dars</a>
                <a href="economics/10-lessons.md#lesson-10">10-dars</a>
            </div>
        </div>

        <div class="card">
            <h2 id="computerTitle">Kompyuter savodxonligi</h2>
            <p id="computerDescription">
                Kompyuter, Windows va internetdan foydalanish asoslarini o'rganing.
            </p>
        </div>

    </div>
</main>

<footer>
    <p id="footerText">
        Student Resources — Talabalar uchun bilim va ta'lim platformasi.
    </p>
</footer>

<script>
const translations = {
    uz: {
        siteTitle: "Student Resources",
        siteDescription: "Talabalar uchun bepul ta'lim platformasi",
        coursesTitle: "O'quv kurslari",
        wordTitle: "Microsoft Word",
        wordDescription: "Matnli hujjatlar yaratish, tahrirlash va bezashni o'rganing.",
        wordLink: "10 ta darsni boshlash",
        excelTitle: "Microsoft Excel",
        excelDescription: "Elektron jadvallar, formulalar va diagrammalar bilan ishlashni o'rganing.",
        excelLink: "10 ta darsni boshlash",
        economicsTitle: "Iqtisodiyot",
        economicsDescription: "Iqtisodiyot fanining asosiy tushunchalari va mavzularini o'rganing.",
        computerTitle: "Kompyuter savodxonligi",
        computerDescription: "Kompyuter, Windows va internetdan foydalanish asoslarini o'rganing.",
        footerText: "Student Resources — Talabalar uchun bilim va ta'lim platformasi.",
        lesson: "dars"
    },
    ru: {
        siteTitle: "Student Resources",
        siteDescription: "Бесплатная образовательная платформа для студентов",
        coursesTitle: "Учебные курсы",
        wordTitle: "Microsoft Word",
        wordDescription: "Научитесь создавать, редактировать и оформлять текстовые документы.",
        wordLink: "Начать 10 уроков",
        excelTitle: "Microsoft Excel",
        excelDescription: "Научитесь работать с электронными таблицами, формулами и диаграммами.",
        excelLink: "Начать 10 уроков",
        economicsTitle: "Экономика",
        economicsDescription: "Изучайте основные понятия и темы экономики.",
        computerTitle: "Компьютерная грамотность",
        computerDescription: "Изучайте основы работы с компьютером, Windows и интернетом.",
        footerText: "Student Resources — образовательная платформа для студентов.",
        lesson: "Урок"
    },
    en: {
        siteTitle: "Student Resources",
        siteDescription: "Free educational platform for students",
        coursesTitle: "Learning Courses",
        wordTitle: "Microsoft Word",
        wordDescription: "Learn to create, edit and format text documents.",
        wordLink: "Start 10 lessons",
        excelTitle: "Microsoft Excel",
        excelDescription: "Learn to work with spreadsheets, formulas and charts.",
        excelLink: "Start 10 lessons",
        economicsTitle: "Economics",
        economicsDescription: "Learn the basic concepts and topics of economics.",
        computerTitle: "Computer Literacy",
        computerDescription: "Learn the basics of computers, Windows and the internet.",
        footerText: "Student Resources — Knowledge and education platform for students.",
        lesson: "Lesson"
    }
};

function changeLanguage(language) {
    const t = translations[language];

    Object.keys(t).forEach(key => {
        if (document.getElementById(key)) {
            document.getElementById(key).textContent = t[key];
        }
    });

    document.querySelectorAll("#economicsLessons a").forEach((link, index) => {
        link.textContent = (index + 1) + "-" + t.lesson;
    });

    document.documentElement.lang = language;
}

changeLanguage("uz");
</script>

</body>
</html>
