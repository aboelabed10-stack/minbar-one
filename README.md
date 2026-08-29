      <!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>منبر ون | منصة الرياضيات</title>

<style>

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:Tahoma,Arial,sans-serif;
}

html{
    scroll-behavior:smooth;
}

body{
    background:#f5f7fb;
    color:#172033;
}

/* NAVBAR */

header{
    position:sticky;
    top:0;
    z-index:1000;

    background:white;
    border-bottom:1px solid #e5e7eb;
}

.nav{
    max-width:1200px;
    margin:auto;

    height:75px;

    display:flex;
    align-items:center;
    justify-content:space-between;

    padding:0 20px;
}

.logo{
    display:flex;
    align-items:center;
    gap:10px;
}

.logo-icon{
    width:45px;
    height:45px;

    display:flex;
    align-items:center;
    justify-content:center;

    border-radius:12px;

    background:linear-gradient(135deg,#3155a6,#172a59);

    color:white;
    font-size:25px;
    font-weight:bold;
}

.logo h2{
    font-size:22px;
}

.logo span{
    display:block;
    font-size:9px;
    color:#64748b;
    letter-spacing:2px;
}

nav{
    display:flex;
    gap:25px;
}

nav a{
    text-decoration:none;
    color:#475569;
    font-size:14px;
}

nav a:hover{
    color:#3155a6;
}

/* HERO */

.hero{
    min-height:620px;

    display:flex;
    align-items:center;

    background:
    radial-gradient(circle at 10% 20%,#dbe5ff,transparent 30%),
    radial-gradient(circle at 90% 80%,#e6edff,transparent 30%),
    linear-gradient(135deg,#fff,#eef3ff);
}

.hero-container{
    max-width:1200px;
    width:92%;
    margin:auto;

    display:grid;
    grid-template-columns:1.2fr .8fr;

    gap:60px;
    align-items:center;
}

.badge{
    display:inline-block;

    padding:8px 15px;

    border-radius:50px;

    background:#e9efff;

    color:#3155a6;

    font-size:13px;

    font-weight:bold;
}

.hero h1{
    font-size:65px;

    line-height:1.1;

    margin:20px 0;
}

.hero h1 span{
    display:block;

    color:#3155a6;
}

.hero p{
    max-width:650px;

    color:#64748b;

    font-size:18px;

    line-height:2;
}

.buttons{
    margin-top:30px;

    display:flex;
    gap:12px;
}

.btn{
    padding:14px 25px;

    border-radius:12px;

    border:none;

    cursor:pointer;

    font-weight:bold;

    font-size:15px;
}

.btn-primary{
    background:#3155a6;
    color:white;
}

.btn-secondary{
    background:white;
    color:#172033;

    border:1px solid #dce2ec;
}

/* MATH CARD */

.math-card{
    min-height:400px;

    border-radius:30px;

    padding:35px;

    color:white;

    background:
    linear-gradient(145deg,#172a59,#3155a6);

    box-shadow:0 25px 60px rgba(23,42,89,.25);

    display:flex;

    flex-direction:column;

    justify-content:center;
}

.math-card small{
    color:#cbd7ff;
}

.formula{
    font-size:34px;
    font-weight:bold;

    margin:30px 0;
}

.math-item{
    background:rgba(255,255,255,.1);

    padding:12px;

    margin:8px 0;

    border-radius:10px;
}

/* FEATURES */

.features{
    padding:70px 0;
}

.container{
    width:92%;
    max-width:1200px;
    margin:auto;
}

.feature-grid{
    display:grid;

    grid-template-columns:repeat(4,1fr);

    gap:20px;
}

.feature{
    background:white;

    padding:30px;

    border-radius:20px;

    border:1px solid #e5e7eb;

    transition:.3s;
}

.feature:hover{
    transform:translateY(-7px);

    box-shadow:0 20px 40px rgba(0,0,0,.08);
}

.feature-icon{
    font-size:40px;
}

.feature h3{
    margin:12px 0 5px;
}

.feature p{
    color:#64748b;

    font-size:14px;
}

/* SECTIONS */

.section{
    padding:80px 0;
}

.section-title{
    margin-bottom:35px;
}

.section-title small{
    color:#3155a6;
    font-weight:bold;
}

.section-title h2{
    font-size:35px;
    margin-top:5px;
}

/* LESSONS */

.lesson-grid{
    display:grid;

    grid-template-columns:repeat(3,1fr);

    gap:20px;
}

.lesson{
    background:white;

    border-radius:20px;

    overflow:hidden;

    border:1px solid #e5e7eb;

    transition:.3s;
}

.lesson:hover{
    transform:translateY(-5px);

    box-shadow:0 20px 40px rgba(0,0,0,.08);
}

.video{
    height:180px;

    background:linear-gradient(135deg,#dce6ff,#eef3ff);

    display:flex;

    align-items:center;
    justify-content:center;

    font-size:55px;

    color:#3155a6;
}

.lesson-body{
    padding:22px;
}

.tag{
    display:inline-block;

    padding:5px 10px;

    border-radius:20px;

    background:#e9efff;

    color:#3155a6;

    font-size:11px;

    font-weight:bold;
}

.lesson h3{
    margin:10px 0 5px;
}

.lesson p{
    color:#64748b;

    font-size:13px;
}

.lesson button{
    margin-top:18px;
}

/* SUMMARIES */

.alt{
    background:#edf2f8;
}

.summary-grid{
    display:grid;

    grid-template-columns:repeat(3,1fr);

    gap:20px;
}

.summary{
    background:white;

    padding:25px;

    border-radius:20px;

    border:1px solid #e5e7eb;
}

.pdf{
    width:55px;
    height:65px;

    background:#e9efff;

    color:#3155a6;

    display:flex;

    align-items:center;
    justify-content:center;

    border-radius:10px;

    font-weight:bold;
}

.summary h3{
    margin:15px 0 5px;
}

.summary p{
    color:#64748b;
}

.summary button{
    margin-top:15px;
}

/* ROOMS */

.room-grid{
    display:grid;

    grid-template-columns:repeat(3,1fr);

    gap:20px;
}

.room{
    background:white;

    padding:28px;

    border-radius:20px;

    border:1px solid #e5e7eb;
}

.room-icon{
    font-size:35px;
}

.room p{
    color:#64748b;

    margin:8px 0;
}

.people{
    font-size:12px;

    color:#64748b;

    margin:15px 0;
}

/* TEST */

.test{
    background:linear-gradient(135deg,#172a59,#3155a6);

    color:white;

    border-radius:25px;

    padding:40px;

    display:flex;

    align-items:center;

    justify-content:space-between;

    gap:20px;
}

.test p{
    color:#d5def4;

    margin-top:8px;
}

/* TEACHER */

.teacher{
    display:grid;

    grid-template-columns:180px 1fr;

    gap:30px;

    align-items:center;
}

.teacher-photo{
    width:180px;
    height:180px;

    border-radius:50%;

    background:#e8eefc;

    display:flex;

    align-items:center;
    justify-content:center;

    font-size:75px;
}

.teacher p{
    color:#64748b;

    max-width:700px;

    margin:10px 0 20px;
}

.phone{
    display:inline-block;

    background:white;

    padding:13px 18px;

    border-radius:10px;

    border:1px solid #e5e7eb;

    margin-bottom:15px;
}

/* CTA */

.cta{
    text-align:center;

    padding:90px 20px;
}

.cta h2{
    font-size:40px;
}

.cta p{
    color:#64748b;

    margin:10px 0 25px;
}

/* FOOTER */

footer{
    background:#101827;

    color:white;

    padding:50px 20px;

    text-align:center;
}

footer h2{
    margin-bottom:8px;
}

footer p{
    color:#9ca9bd;
}

.footer-links{
    margin:20px 0;

    display:flex;

    justify-content:center;

    gap:20px;
}

.footer-links a{
    color:#c5cede;

    text-decoration:none;

    font-size:13px;
}

/* MOBILE */

@media(max-width:900px){

    nav{
        display:none;
    }

    .hero-container{
        grid-template-columns:1fr;
    }

    .math-card{
        display:none;
    }

    .feature-grid{
        grid-template-columns:repeat(2,1fr);
    }

    .lesson-grid,
    .summary-grid,
    .room-grid{
        grid-template-columns:1fr 1fr;
    }

}

@media(max-width:600px){

    .hero{
        padding:60px 0;
    }

    .hero h1{
        font-size:42px;
    }

    .hero p{
        font-size:16px;
    }

    .feature-grid,
    .lesson-grid,
    .summary-grid,
    .room-grid{
        grid-template-columns:1fr;
    }

    .teacher{
        grid-template-columns:1fr;

        text-align:center;
    }

    .teacher-photo{
        margin:auto;
    }

    .test{
        flex-direction:column;

        align-items:flex-start;
    }

}

</style>
</head>

<body>

<!-- HEADER -->

<header>

<div class="nav">

<div class="logo">

<div class="logo-icon">
∑
</div>

<div>
<h2>منبر ون</h2>
<span>MINBAR ONE</span>
</div>

</div>

<nav>

<a href="#home">الرئيسية</a>

<a href="#lessons">الحصص</a>

<a href="#summaries">الملخصات</a>

<a href="#rooms">الرومات</a>

<a href="#tests">الاختبارات</a>

<a href="#teacher">الأستاذ</a>

</nav>

</div>

</header>


<!-- HERO -->

<section class="hero" id="home">

<div class="hero-container">

<div>

<span class="badge">
🎓 منصة الرياضيات لطلاب التوجيهي
</span>

<h1>
الرياضيات أصبحت
<span>أسهل مع منبر ون</span>
</h1>

<p>

منصة تعليمية متخصصة لطلاب التوجيهي.
حصص فيديو، ملخصات، رومات، اختبارات
وكل ما تحتاجه لتطوير مستواك في الرياضيات.

</p>

<div class="buttons">

<button class="btn btn-primary"
onclick="document.getElementById('lessons').scrollIntoView()">

🚀 ابدأ التعلم

</button>

<button class="btn btn-secondary"
onclick="document.getElementById('tests').scrollIntoView()">

📝 اختبر نفسك

</button>

</div>

</div>


<div class="math-card">

<small>
منبر ون • رياضيات التوجيهي
</small>

<div class="formula">
f(x) = x² + 2x + 1
</div>

<div class="math-item">
📌 افهم الفكرة
</div>

<div class="math-item">
✏️ حل بنفسك
</div>

<div class="math-item">
🏆 اختبر مستواك
</div>

</div>

</div>

</section>


<!-- FEATURES -->

<section class="features">

<div class="container">

<div class="feature-grid">

<div class="feature">

<div class="feature-icon">
🎥
</div>

<h3>
الحصص
</h3>

<p>
حصص فيديو مرتبة حسب الوحدات والدروس.
</p>

</div>


<div class="feature">

<div class="feature-icon">
📚
</div>

<h3>
الملخصات
</h3>

<p>
ملخصات وقوانين تساعدك على المراجعة.
</p>

</div>


<div class="feature">

<div class="feature-icon">
💬
</div>

<h3>
الرومات
</h3>

<p>
رومات تعليمية للنقاش وطرح الأسئلة.
</p>

</div>


<div class="feature">

<div class="feature-icon">
📝
</div>

<h3>
الاختبارات
</h3>

<p>
اختبارات تدريبية لمعرفة مستواك.
</p>

</div>

</div>

</div>

</section>


<!-- LESSONS -->

<section class="section" id="lessons">

<div class="container">

<div class="section-title">

<small>
تعلم خطوة بخطوة
</small>

<h2>
🎥 الحصص التعليمية
</h2>

</div>


<div class="lesson-grid">


<div class="lesson">

<div class="video">
▶
</div>

<div class="lesson-body">

<span class="tag">
الوحدة الأولى
</span>

<h3>
مقدمة في الرياضيات
</h3>

<p>
شرح المفاهيم الأساسية للطلاب.
</p>

<button
class="btn btn-primary"
onclick="alert('سيتم ربط الفيديو الحقيقي هنا')">

مشاهدة الحصة

</button>

</div>

</div>



<div class="lesson">

<div class="video">
▶
</div>

<div class="lesson-body">

<span class="tag">
الوحدة الأولى
</span>

<h3>
الدوال
</h3>

<p>
شرح الدوال بطريقة سهلة مع أمثلة.
</p>

<button
class="btn btn-primary"
onclick="alert('سيتم ربط الفيديو الحقيقي هنا')">

مشاهدة الحصة

</button>

</div>

</div>



<div class="lesson">

<div class="video">
▶
</div>

<div class="lesson-body">

<span class="tag">
الوحدة الثانية
</span>

<h3>
التفاضل
</h3>

<p>
شرح أساسيات التفاضل وتطبيقاته.
</p>

<button
class="btn btn-primary"
onclick="alert('سيتم ربط الفيديو الحقيقي هنا')">

مشاهدة الحصة

</button>

</div>

</div>


</div>

</div>

</section>


<!-- SUMMARIES -->

<section class="section alt" id="summaries">

<div class="container">

<div class="section-title">

<small>
مكتبة منبر ون
</small>

<h2>
📚 الملخصات والملفات
</h2>

</div>


<div class="summary-grid">


<div class="summary">

<div class="pdf">
PDF
</div>

<h3>
ملخص الوحدة الأولى
</h3>

<p>
أهم القوانين والأفكار.
</p>

<button
class="btn btn-primary"
onclick="alert('سيتم ربط ملف PDF هنا')">

فتح الملخص

</button>

</div>


<div class="summary">

<div class="pdf">
PDF
</div>

<h3>
القوانين المهمة
</h3>

<p>
ورقة مراجعة سريعة.
</p>

<button
class="btn btn-primary"
onclick="alert('سيتم ربط ملف PDF هنا')">

فتح الملف

</button>

</div>


<div class="summary">

<div class="pdf">
PDF
</div>

<h3>
نموذج امتحان
</h3>

<p>
نموذج تدريبي لطلاب التوجيهي.
</p>

<button
class="btn btn-primary"
onclick="alert('سيتم ربط ملف PDF هنا')">

فتح النموذج

</button>

</div>


</div>

</div>

</section>


<!-- ROOMS -->

<section class="section" id="rooms">

<div class="container">

<div class="section-title">

<small>
مجتمع منبر ون
</small>

<h2>
💬 الرومات التعليمية
</h2>

</div>


<div class="room-grid">


<div class="room">

<div class="room-icon">
🟢
</div>

<h3>
روم الرياضيات العام
</h3>

<p>
ناقش الأسئلة مع الطلاب.
</p>

<div class="people">
👥 245 طالب
</div>

<button
class="btn btn-primary"
onclick="alert('سيتم فتح الروم هنا')">

دخول الروم

</button>

</div>



<div class="room">

<div class="room-icon">
🔵
</div>

<h3>
روم المراجعة
</h3>

<p>
مراجعة الدروس وحل الأسئلة.
</p>

<div class="people">
👥 180 طالب
</div>

<button
class="btn btn-primary"
onclick="alert('سيتم فتح الروم هنا')">

دخول الروم

</button>

</div>



<div class="room">

<div class="room-icon">
🟣
</div>

<h3>
روم الأسئلة
</h3>

<p>
اطرح سؤالك وناقشه.
</p>

<div class="people">
👥 120 طالب
</div>

<button
class="btn btn-primary"
onclick="alert('سيتم فتح الروم هنا')">

دخول الروم

</button>

</div>


</div>

</div>

</section>


<!-- TESTS -->

<section class="section alt" id="tests">

<div class="container">

<div class="test">

<div>

<h2>
📝 اختبر مستواك
</h2>

<p>
اختبارات تدريبية تساعدك على معرفة نقاط قوتك وضعفك.
</p>

</div>

<button
class="btn btn-secondary"
onclick="alert('سيتم فتح الاختبار هنا')">

ابدأ الاختبار 🚀

</button>

</div>

</div>

</section>


<!-- TEACHER -->

<section class="section" id="teacher">

<div class="container">

<div class="teacher">

<div class="teacher-photo">
👨‍🏫
</div>

<div>

<small style="color:#3155a6;font-weight:bold">
المدرس
</small>

<h2>
الأستاذ
</h2>

<p>

شرح مبسط ومنظم لمادة الرياضيات،
مع متابعة ومراجعة واختبارات تدريبية
لطلاب التوجيهي.

</p>

<div class="phone">

📞 رقم الأستاذ:
<strong>
ضع الرقم هنا
</strong>

</div>

<br>

<button
class="btn btn-primary"
onclick="alert('ضع رقم الأستاذ الحقيقي في الكود')">

تواصل مع الأستاذ

</button>

</div>

</div>

</div>

</section>


<!-- CTA -->

<section class="cta">

<h2>
جاهز تبدأ؟ 🚀
</h2>

<p>
اجعل الرياضيات أسهل مع منبر ون.
</p>

<button
class="btn btn-primary"
onclick="document.getElementById('lessons').scrollIntoView()">

ابدأ التعلم الآن

</button>

</section>


<!-- FOOTER -->

<footer>

<h2>
منبر ون
</h2>

<p>
منصة الرياضيات لطلاب التوجيهي
</p>

<div class="footer-links">

<a href="#home">
الرئيسية
</a>

<a href="#lessons">
الحصص
</a>

<a href="#summaries">
الملخصات
</a>

<a href="#rooms">
الرومات
</a>

<a href="#tests">
الاختبارات
</a>

</div>

<p>
© 2026 منبر ون — جميع الحقوق محفوظة
</p>

</footer>

</body>
</html>
