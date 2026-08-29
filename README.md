<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>منبر ون | الرياضيات بطريقة مختلفة</title>

<style>
:root{
  --blue:#4f7cff;
  --purple:#7c5cff;
  --yellow:#ffc83d;
  --green:#32c48d;
  --pink:#ff6b9d;
  --dark:#17213a;
  --text:#202b45;
  --muted:#718096;
  --bg:#f7f9ff;
  --white:#fff;
  --border:#e7ebf5;
  --shadow:0 15px 40px rgba(48,67,120,.10);
}

*{
  box-sizing:border-box;
  margin:0;
  padding:0;
}

html{
  scroll-behavior:smooth;
}

body{
  font-family:Tahoma,Arial,sans-serif;
  background:var(--bg);
  color:var(--text);
  line-height:1.7;
}

/* ===== HEADER ===== */

header{
  position:sticky;
  top:0;
  z-index:1000;
  background:rgba(255,255,255,.94);
  backdrop-filter:blur(15px);
  border-bottom:1px solid var(--border);
}

.nav{
  max-width:1200px;
  width:92%;
  height:75px;
  margin:auto;

  display:flex;
  align-items:center;
  justify-content:space-between;
}

.logo{
  display:flex;
  align-items:center;
  gap:10px;
}

.logo-icon{
  width:48px;
  height:48px;
  border-radius:15px;

  display:grid;
  place-items:center;

  color:white;
  font-size:25px;
  font-weight:bold;

  background:linear-gradient(135deg,var(--blue),var(--purple));

  box-shadow:0 8px 20px rgba(79,124,255,.25);
}

.logo h2{
  font-size:21px;
}

.logo span{
  display:block;
  font-size:9px;
  color:var(--muted);
  letter-spacing:2px;
}

nav{
  display:flex;
  gap:22px;
}

nav a{
  color:#526078;
  text-decoration:none;
  font-size:13px;
  transition:.2s;
}

nav a:hover{
  color:var(--blue);
}

.nav-button{
  background:var(--blue);
  color:white;
  border:0;
  border-radius:11px;
  padding:10px 16px;
  cursor:pointer;
  font-weight:bold;
}

/* ===== HERO ===== */

.hero{
  position:relative;
  overflow:hidden;

  padding:75px 0;

  background:
  radial-gradient(circle at 10% 20%,#dfe8ff,transparent 30%),
  radial-gradient(circle at 90% 80%,#eee5ff,transparent 30%),
  linear-gradient(135deg,#ffffff,#f0f4ff);
}

.hero-container{
  max-width:1200px;
  width:92%;
  margin:auto;

  display:grid;
  grid-template-columns:1.1fr .9fr;

  align-items:center;
  gap:50px;
}

.date-box{
  display:inline-flex;
  align-items:center;
  gap:8px;

  background:white;
  padding:8px 14px;

  border-radius:30px;

  color:#5d6980;

  font-size:12px;

  box-shadow:0 5px 20px rgba(50,70,120,.07);
}

.hero h1{
  font-size:clamp(42px,6vw,68px);
  line-height:1.12;

  margin:20px 0;
}

.hero h1 span{
  color:var(--blue);
}

.hero p{
  color:var(--muted);
  max-width:650px;
  font-size:17px;
}

.buttons{
  display:flex;
  gap:12px;
  margin-top:28px;
}

.btn{
  border:0;
  border-radius:12px;
  padding:13px 20px;
  cursor:pointer;
  font-weight:bold;
  transition:.2s;
}

.btn:hover{
  transform:translateY(-3px);
}

.primary{
  background:var(--blue);
  color:white;
  box-shadow:0 10px 25px rgba(79,124,255,.22);
}

.secondary{
  background:white;
  color:var(--text);
  border:1px solid var(--border);
}

/* ===== MATH ILLUSTRATION ===== */

.math-board{
  position:relative;

  min-height:410px;

  background:white;

  border-radius:30px;

  box-shadow:var(--shadow);

  padding:35px;

  overflow:hidden;
}

.math-board:before{
  content:"";

  position:absolute;

  width:200px;
  height:200px;

  background:#e8edff;

  border-radius:50%;

  top:-80px;
  right:-70px;
}

.math-title{
  position:relative;
  z-index:1;

  color:var(--muted);
  font-size:13px;
}

.equation{
  position:relative;
  z-index:1;

  margin:35px 0;

  text-align:center;

  font-size:38px;

  font-weight:bold;

  color:var(--purple);
}

.math-symbols{
  display:grid;

  grid-template-columns:repeat(3,1fr);

  gap:12px;

  position:relative;
  z-index:1;
}

.symbol{
  height:80px;

  border-radius:17px;

  display:grid;
  place-items:center;

  font-size:28px;
  font-weight:bold;

  color:var(--dark);
}

.symbol:nth-child(1){
  background:#fff1b8;
}

.symbol:nth-child(2){
  background:#dff8ee;
}

.symbol:nth-child(3){
  background:#ffe0ec;
}

.symbol:nth-child(4){
  background:#e2eaff;
}

.symbol:nth-child(5){
  background:#eee4ff;
}

.symbol:nth-child(6){
  background:#dff5ff;
}

/* ===== CONTAINER ===== */

.container{
  width:92%;
  max-width:1200px;
  margin:auto;
}

/* ===== MOTIVATION ===== */

.motivation{
  padding:35px 0;
}

.motivation-box{
  background:linear-gradient(135deg,var(--purple),var(--blue));

  color:white;

  border-radius:25px;

  padding:30px;

  display:flex;

  align-items:center;

  justify-content:space-between;

  gap:20px;

  box-shadow:var(--shadow);
}

.motivation-box p{
  color:#e5e9ff;
}

.quote{
  font-size:40px;
}

/* ===== DAILY PLAN ===== */

.section{
  padding:75px 0;
}

.section-title{
  margin-bottom:30px;
}

.section-title small{
  color:var(--blue);
  font-weight:bold;
}

.section-title h2{
  font-size:32px;
  margin-top:5px;
}

.plan{
  display:grid;

  grid-template-columns:repeat(3,1fr);

  gap:18px;
}

.plan-card{
  background:white;

  padding:24px;

  border-radius:20px;

  border:1px solid var(--border);

  box-shadow:0 6px 20px rgba(40,60,100,.04);

  transition:.25s;
}

.plan-card:hover{
  transform:translateY(-5px);
  box-shadow:var(--shadow);
}

.plan-icon{
  font-size:38px;
}

.plan-card h3{
  margin:10px 0 4px;
}

.plan-card p{
  color:var(--muted);
  font-size:13px;
}

.progress{
  height:8px;

  background:#edf0f6;

  border-radius:20px;

  margin:15px 0 8px;

  overflow:hidden;
}

.progress span{
  display:block;
  height:100%;
  width:70%;

  background:linear-gradient(90deg,var(--blue),var(--purple));
}

.plan-card button{
  margin-top:8px;
}

/* ===== FEATURES ===== */

.features{
  background:#eef3ff;
}

.feature-grid{
  display:grid;

  grid-template-columns:repeat(4,1fr);

  gap:18px;
}

.feature{
  background:white;

  padding:25px;

  border-radius:20px;

  text-align:center;

  border:1px solid var(--border);

  transition:.2s;
}

.feature:hover{
  transform:translateY(-5px);
}

.feature-icon{
  font-size:40px;
}

.feature h3{
  margin:8px 0 4px;
}

.feature p{
  color:var(--muted);
  font-size:13px;
}

/* ===== LESSONS ===== */

.lesson-grid{
  display:grid;

  grid-template-columns:repeat(3,1fr);

  gap:20px;
}

.lesson{
  background:white;

  border-radius:20px;

  overflow:hidden;

  border:1px solid var(--border);

  transition:.2s;
}

.lesson:hover{
  transform:translateY(-5px);
  box-shadow:var(--shadow);
}

.video{
  height:180px;

  display:grid;
  place-items:center;

  font-size:55px;

  background:linear-gradient(135deg,#dfe8ff,#eee6ff);

  color:var(--blue);
}

.lesson-body{
  padding:22px;
}

.tag{
  display:inline-block;

  padding:5px 10px;

  border-radius:20px;

  background:#eaf0ff;

  color:var(--blue);

  font-size:11px;

  font-weight:bold;
}

.lesson h3{
  margin:10px 0 5px;
}

.lesson p{
  color:var(--muted);
  font-size:13px;
}

/* ===== SUMMARIES ===== */

.alt{
  background:#f0f3f9;
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

  border:1px solid var(--border);

  transition:.2s;
}

.summary:hover{
  transform:translateY(-5px);
}

.pdf{
  width:58px;
  height:68px;

  display:grid;
  place-items:center;

  border-radius:12px;

  background:#ffe5ec;

  color:#d94f78;

  font-weight:bold;
}

/* ===== ROOMS ===== */

.room-grid{
  display:grid;

  grid-template-columns:repeat(3,1fr);

  gap:20px;
}

.room{
  background:white;

  padding:27px;

  border-radius:20px;

  border:1px solid var(--border);
}

.room-icon{
  font-size:35px;
}

.room p{
  color:var(--muted);

  font-size:13px;
}

.people{
  color:var(--muted);

  font-size:12px;

  margin:15px 0;
}

/* ===== TEST ===== */

.test{
  background:linear-gradient(135deg,#16234a,#4f7cff);

  color:white;

  border-radius:25px;

  padding:40px;

  display:flex;

  align-items:center;

  justify-content:space-between;

  gap:20px;
}

.test p{
  color:#dbe3ff;

  margin-top:8px;
}

/* ===== TEACHER ===== */

.teacher{
  display:grid;

  grid-template-columns:180px 1fr;

  gap:35px;

  align-items:center;
}

.teacher-photo{
  width:180px;
  height:180px;

  border-radius:50%;

  display:grid;
  place-items:center;

  font-size:75px;

  background:linear-gradient(135deg,#ffe8a7,#ffd6e6);
}

.teacher p{
  color:var(--muted);

  max-width:700px;

  margin:10px 0 20px;
}

.phone{
  display:inline-block;

  padding:12px 18px;

  background:white;

  border:1px solid var(--border);

  border-radius:11px;
}

/* ===== CTA ===== */

.cta{
  text-align:center;

  padding:90px 20px;

  background:
  radial-gradient(circle at 20% 50%,#e0e8ff,transparent 30%),
  white;
}

.cta h2{
  font-size:40px;
}

.cta p{
  color:var(--muted);

  margin:10px 0 25px;
}

/* ===== FOOTER ===== */

footer{
  background:#121a2e;

  color:white;

  padding:50px 20px;

  text-align:center;
}

footer p{
  color:#9eabc1;

  font-size:13px;
}

.footer-links{
  display:flex;

  justify-content:center;

  gap:20px;

  margin:20px 0;
}

.footer-links a{
  color:#c7d0e0;

  text-decoration:none;

  font-size:13px;
}

/* ===== MOBILE ===== */

@media(max-width:900px){

  nav{
    display:none;
  }

  .hero-container{
    grid-template-columns:1fr;
  }

  .math-board{
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

  .nav{
    height:65px;
  }

  .hero{
    padding:55px 0;
  }

  .hero h1{
    font-size:42px;
  }

  .buttons{
    flex-direction:column;
  }

  .buttons .btn{
    width:100%;
  }

  .motivation-box{
    flex-direction:column;
    align-items:flex-start;
  }

  .plan,
  .feature-grid,
  .lesson-grid,
  .summary-grid,
  .room-grid{
    grid-template-columns:1fr;
  }

  .section{
    padding:55px 0;
  }

  .test{
    flex-direction:column;
    align-items:flex-start;
  }

  .teacher{
    grid-template-columns:1fr;
    text-align:center;
  }

  .teacher-photo{
    margin:auto;
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

<a href="#plan">خطتي</a>

<a href="#lessons">الحصص</a>

<a href="#summaries">الملخصات</a>

<a href="#rooms">الرومات</a>

<a href="#tests">الاختبارات</a>

<a href="#teacher">الأستاذ</a>

</nav>


<button
class="nav-button"
onclick="login()">

دخول الطالب 👤

</button>

</div>

</header>



<!-- HERO -->

<section class="hero" id="home">

<div class="hero-container">


<div>

<div class="date-box">

📅

<span id="date">
اليوم
</span>

</div>


<h1>

صباح الخير 👋

<br>

<span>يا بطل الرياضيات!</span>

</h1>


<p>

جاهز ننجز درس اليوم؟ 🚀

كل حصة تحضرها وكل سؤال تحله
يقرّبك أكثر من هدفك 🎯

</p>


<div class="buttons">

<button
class="btn primary"
onclick="goTo('plan')">

🚀 خطتي اليوم

</button>


<button
class="btn secondary"
onclick="goTo('lessons')">

🎥 ابدأ حصة

</button>

</div>

</div>



<!-- MATH -->

<div class="math-board">

<div class="math-title">

🧮 لوحة الرياضيات

</div>


<div class="equation">

x² + 2x + 1

</div>


<div class="math-symbols">

<div class="symbol">
π
</div>

<div class="symbol">
√
</div>

<div class="symbol">
∑
</div>

<div class="symbol">
x²
</div>

<div class="symbol">
∞
</div>

<div class="symbol">
÷
</div>

</div>

</div>

</div>

</section>



<!-- MOTIVATION -->

<section class="motivation">

<div class="container">

<div class="motivation-box">

<div>

<h2>
🔥 استمر... أنت قادر!
</h2>

<p>
لا تحتاج أن تكون عبقريًا في الرياضيات،
تحتاج فقط أن تستمر.
</p>

</div>

<div class="quote">
🎯
</div>

</div>

</div>

</section>



<!-- DAILY PLAN -->

<section class="section" id="plan">

<div class="container">

<div class="section-title">

<small>
خطة اليوم
</small>

<h2>
📅 ماذا سننجز اليوم؟
</h2>

</div>


<div class="plan">


<div class="plan-card">

<div class="plan-icon">
🎥
</div>

<h3>
حصة الدوال
</h3>

<p>
شرح + أمثلة تطبيقية
</p>

<div class="progress">
<span style="width:70%"></span>
</div>

<small>
70% من الخطة
</small>

<br>

<button
class="btn primary"
onclick="alert('سيتم فتح الفيديو هنا')">

ابدأ الحصة

</button>

</div>



<div class="plan-card">

<div class="plan-icon">
📝
</div>

<h3>
اختبار سريع
</h3>

<p>
10 أسئلة لتقييم مستواك
</p>

<div class="progress">
<span style="width:40%"></span>
</div>

<small>
لم تبدأ بعد
</small>

<br>

<button
class="btn primary"
onclick="alert('سيتم فتح الاختبار هنا')">

ابدأ الاختبار

</button>

</div>



<div class="plan-card">

<div class="plan-icon">
📖
</div>

<h3>
مراجعة القوانين
</h3>

<p>
15 دقيقة مراجعة
</p>

<div class="progress">
<span style="width:85%"></span>
</div>

<small>
85% مكتمل
</small>

<br>

<button
class="btn primary"
onclick="alert('سيتم فتح الملخص هنا')">

راجع الآن

</button>

</div>


</div>

</div>

</section>



<!-- FEATURES -->

<section class="section features">

<div class="container">

<div class="section-title">

<small>
كل ما تحتاجه
</small>

<h2>
🚀 منبر ون في مكان واحد
</h2>

</div>


<div class="feature-grid">


<div class="feature">

<div class="feature-icon">
🎥
</div>

<h3>
حصص فيديو
</h3>

<p>
تعلم من خلال حصص مرتبة وسهلة.
</p>

</div>


<div class="feature">

<div class="feature-icon">
📚
</div>

<h3>
ملخصات
</h3>

<p>
القوانين والأفكار المهمة في مكان واحد.
</p>

</div>


<div class="feature">

<div class="feature-icon">
💬
</div>

<h3>
رومات
</h3>

<p>
اسأل وناقش وتعلم مع زملائك.
</p>

</div>


<div class="feature">

<div class="feature-icon">
🏆
</div>

<h3>
اختبارات
</h3>

<p>
اختبر نفسك وتابع تقدمك.
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
تعلم بطريقة أسهل
</small>

<h2>
🎥 أحدث الحصص
</h2>

</div>


<div class="lesson-grid">


<div class="lesson">

<div class="video">
▶️
</div>

<div class="lesson-body">

<span class="tag">
الوحدة الأولى
</span>

<h3>
الدوال
</h3>

<p>
شرح الدوال مع أمثلة وتطبيقات.
</p>

<button
class="btn primary"
onclick="alert('سيتم تشغيل الفيديو هنا')">

مشاهدة الحصة

</button>

</div>

</div>



<div class="lesson">

<div class="video">
▶️
</div>

<div class="lesson-body">

<span class="tag">
الوحدة الثانية
</span>

<h3>
التفاضل
</h3>

<p>
أساسيات التفاضل بطريقة مبسطة.
</p>

<button
class="btn primary"
onclick="alert('سيتم تشغيل الفيديو هنا')">

مشاهدة الحصة

</button>

</div>

</div>



<div class="lesson">

<div class="video">
▶️
</div>

<div class="lesson-body">

<span class="tag">
الوحدة الثالثة
</span>

<h3>
التكامل
</h3>

<p>
شرح التكامل وأهم القوانين.
</p>

<button
class="btn primary"
onclick="alert('سيتم تشغيل الفيديو هنا')">

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
مكتبة الطالب
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
class="btn primary"
onclick="alert('سيتم فتح ملف PDF هنا')">

فتح الملخص

</button>

</div>



<div class="summary">

<div class="pdf">
PDF
</div>

<h3>
ورقة القوانين
</h3>

<p>
مراجعة سريعة قبل الاختبار.
</p>

<button
class="btn primary"
onclick="alert('سيتم فتح الملف هنا')">

فتح الملف

</button>

</div>



<div class="summary">

<div class="pdf">
PDF
</div>

<h3>
نماذج امتحانات
</h3>

<p>
نماذج تدريبية للتوجيهي.
</p>

<button
class="btn primary"
onclick="alert('سيتم فتح النموذج هنا')">

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
تعلم مع الآخرين
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
ناقش الأسئلة مع زملائك.
</p>

<div class="people">
👥 245 طالب
</div>

<button
class="btn primary"
onclick="alert('سيتم دخول الروم هنا')">

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
class="btn primary"
onclick="alert('سيتم دخول الروم هنا')">

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
اسأل عن أي سؤال لم تفهمه.
</p>

<div class="people">
👥 120 طالب
</div>

<button
class="btn primary"
onclick="alert('سيتم دخول الروم هنا')">

دخول الروم

</button>

</div>


</div>

</div>

</section>



<!-- TEST -->

<section class="section alt" id="tests">

<div class="container">

<div class="test">

<div>

<h2>
📝 اختبر مستواك
</h2>

<p>
هل أنت مستعد؟ جرّب اختبارًا سريعًا الآن.
</p>

</div>

<button
class="btn secondary"
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

<small style="color:#4f7cff;font-weight:bold">
مدرس الرياضيات
</small>

<h2>
الأستاذ
</h2>

<p>

هنا يمكن وضع اسم الأستاذ،
نبذة عنه، والخبرات وطريقة التواصل معه.

</p>

<div class="phone">

📞 رقم الأستاذ:

<strong>
ضع الرقم هنا
</strong>

</div>

<br><br>

<button
class="btn primary"
onclick="alert('ضع رقم الأستاذ الحقيقي هنا')">

تواصل مع الأستاذ

</button>

</div>

</div>

</div>

</section>



<!-- CTA -->

<section class="cta">

<h2>
🚀 مستعد تحقق هدفك؟
</h2>

<p>
ابدأ اليوم، ولا تؤجل نجاحك إلى الغد.
</p>

<button
class="btn primary"
onclick="goTo('lessons')">

ابدأ التعلم الآن 📚

</button>

</section>



<!-- FOOTER -->

<footer>

<h2>
∑ منبر ون
</h2>

<p>
منصة الرياضيات لطلاب التوجيهي 🎓
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



<script>

/* التاريخ */

const today = new Date();

const days = [
"الأحد",
"الاثنين",
"الثلاثاء",
"الأربعاء",
"الخميس",
"الجمعة",
"السبت"
];

const months = [
"يناير",
"فبراير",
"مارس",
"أبريل",
"مايو",
"يونيو",
"يوليو",
"أغسطس",
"سبتمبر",
"أكتوبر",
"نوفمبر",
"ديسمبر"
];

document.getElementById("date").innerText =
days[today.getDay()] +
" • " +
today.getDate() +
" " +
months[today.getMonth()] +
" " +
today.getFullYear();


/* الانتقال */

function goTo(id){

document.getElementById(id).scrollIntoView({
behavior:"smooth"
});

}


/* تسجيل الدخول التجريبي */

function login(){

alert(
"👋 أهلاً بك في منبر ون!\n\n" +
"سيتم إضافة نظام تسجيل دخول حقيقي للطلاب في المرحلة القادمة."
);

}

</script>

</body>
</html>
