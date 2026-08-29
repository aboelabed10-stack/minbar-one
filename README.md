# minbar-one
منصة منبر ون التعليمية للرياضيات وطلاب التوجيهي
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <title>منبر ون | منصة الرياضيات للتوجيهي</title>

  <link rel="stylesheet" href="style.css">
</head>

<body>

<header class="navbar">

  <div class="logo">
    <span class="logo-icon">∑</span>
    <div>
      <strong>منبر ون</strong>
      <small>MINBAR ONE</small>
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

  <div class="nav-actions">
    <button onclick="toggleDarkMode()" class="icon-btn">🌙</button>
    <button onclick="openLogin()" class="login-btn">دخول الطالب</button>
  </div>

</header>


<main>

<section id="home" class="hero">

  <div class="hero-content">

    <div class="badge">🎓 منصة الرياضيات لطلاب التوجيهي</div>

    <h1>
      الرياضيات أصبحت
      <span>أسهل مع منبر ون</span>
    </h1>

    <p>
      حصص، ملخصات، اختبارات ورومات تعليمية
      تساعدك على فهم الرياضيات والاستعداد للامتحان.
    </p>

    <div class="hero-buttons">
      <button class="primary-btn" onclick="scrollToSection('lessons')">
        🚀 ابدأ التعلم
      </button>

      <button class="secondary-btn" onclick="scrollToSection('tests')">
        📝 اختبر نفسك
      </button>
    </div>

    <div class="hero-stats">

      <div>
        <strong>100+</strong>
        <span>حصة تعليمية</span>
      </div>

      <div>
        <strong>500+</strong>
        <span>سؤال تدريبي</span>
      </div>

      <div>
        <strong>50+</strong>
        <span>ملخص ونموذج</span>
      </div>

    </div>

  </div>

  <div class="hero-card">

    <div class="math-display">
      <span>رياضيات التوجيهي</span>

      <div class="formula">
        f(x) = x² + 2x + 1
      </div>

      <p>افهمها • تدرب عليها • أتقنها</p>
    </div>

  </div>

</section>


<section class="features">

  <div class="feature-card">
    <div>🎥</div>
    <h3>حصص مسجلة</h3>
    <p>شرح منظم وسهل لجميع الدروس.</p>
  </div>

  <div class="feature-card">
    <div>📚</div>
    <h3>ملخصات</h3>
    <p>ملخصات وقوانين تساعدك على المراجعة.</p>
  </div>

  <div class="feature-card">
    <div>📝</div>
    <h3>اختبارات</h3>
    <p>اختبر نفسك واعرف مستواك.</p>
  </div>

  <div class="feature-card">
    <div>💬</div>
    <h3>رومات</h3>
    <p>تواصل ومناقشة الأسئلة.</p>
  </div>

</section>


<section id="lessons" class="section">

  <div class="section-title">

    <div>
      <span>تعلم معنا</span>
      <h2>🎥 الحصص التعليمية</h2>
    </div>

    <input
      id="lessonSearch"
      onkeyup="searchLessons()"
      placeholder="🔎 ابحث عن حصة..."
    >

  </div>


  <div class="filter-buttons">
    <button onclick="filterLessons('all')">الكل</button>
    <button onclick="filterLessons('1')">الوحدة الأولى</button>
    <button onclick="filterLessons('2')">الوحدة الثانية</button>
    <button onclick="filterLessons('3')">الوحدة الثالثة</button>
  </div>


  <div class="cards" id="lessonsContainer">

    <article class="lesson-card" data-unit="1">

      <div class="video-placeholder">
        ▶
      </div>

      <div class="card-body">

        <span class="tag">الوحدة الأولى</span>

        <h3>مقدمة في الرياضيات</h3>

        <p>
          شرح تمهيدي للمفاهيم الأساسية.
        </p>

        <div class="card-footer">
          <span>⏱️ 35 دقيقة</span>
          <button onclick="playLesson('مقدمة في الرياضيات')">
            مشاهدة
          </button>
        </div>

      </div>

    </article>


    <article class="lesson-card" data-unit="1">

      <div class="video-placeholder">
        ▶
      </div>

      <div class="card-body">

        <span class="tag">الوحدة الأولى</span>

        <h3>الدوال</h3>

        <p>
          شرح الدوال وأهم القوانين والأمثلة.
        </p>

        <div class="card-footer">
          <span>⏱️ 42 دقيقة</span>
          <button onclick="playLesson('الدوال')">
            مشاهدة
          </button>
        </div>

      </div>

    </article>


    <article class="lesson-card" data-unit="2">

      <div class="video-placeholder">
        ▶
      </div>

      <div class="card-body">

        <span class="tag">الوحدة الثانية</span>

        <h3>التفاضل</h3>

        <p>
          فهم أساسيات التفاضل بطريقة سهلة.
        </p>

        <div class="card-footer">
          <span>⏱️ 48 دقيقة</span>
          <button onclick="playLesson('التفاضل')">
            مشاهدة
          </button>
        </div>

      </div>

    </article>


    <article class="lesson-card" data-unit="3">

      <div class="video-placeholder">
        ▶
      </div>

      <div class="card-body">

        <span class="tag">الوحدة الثالثة</span>

        <h3>التكامل</h3>

        <p>
          شرح مبسط للتكامل مع أمثلة.
        </p>

        <div class="card-footer">
          <span>⏱️ 50 دقيقة</span>
          <button onclick="playLesson('التكامل')">
            مشاهدة
          </button>
        </div>

      </div>

    </article>

  </div>

</section>


<section id="summaries" class="section alt-section">

  <div class="section-title">
    <div>
      <span>مكتبة منبر ون</span>
      <h2>📚 الملخصات والملفات</h2>
    </div>
  </div>


  <div class="cards">

    <div class="summary-card">
      <div class="file-icon">PDF</div>

      <h3>ملخص الوحدة الأولى</h3>

      <p>أهم القوانين والأفكار.</p>

      <button onclick="openFile('ملخص الوحدة الأولى')">
        فتح الملخص
      </button>
    </div>


    <div class="summary-card">
      <div class="file-icon">PDF</div>

      <h3>القوانين المهمة</h3>

      <p>ورقة مراجعة سريعة.</p>

      <button onclick="openFile('القوانين المهمة')">
        فتح الملخص
      </button>
    </div>


    <div class="summary-card">
      <div class="file-icon">PDF</div>

      <h3>نموذج امتحان</h3>

      <p>اختبار تدريبي للتوجيهي.</p>

      <button onclick="openFile('نموذج امتحان')">
        فتح الملف
      </button>
    </div>

  </div>

</section>


<section id="rooms" class="section">

  <div class="section-title">
    <div>
      <span>مجتمع منبر ون</span>
      <h2>💬 الرومات التعليمية</h2>
    </div>
  </div>


  <div class="rooms-grid">

    <div class="room-card">
      <div class="room-icon">🟢</div>

      <h3>روم الرياضيات العام</h3>

      <p>
        مكان لمناقشة الأسئلة والاستفسارات.
      </p>

      <span>👥 245 طالب</span>

      <button onclick="joinRoom('روم الرياضيات العام')">
        دخول الروم
      </button>
    </div>


    <div class="room-card">
      <div class="room-icon">🔵</div>

      <h3>روم المراجعة</h3>

      <p>
        مراجعة الدروس وحل الأسئلة.
      </p>

      <span>👥 180 طالب</span>

      <button onclick="joinRoom('روم المراجعة')">
        دخول الروم
      </button>
    </div>


    <div class="room-card">
      <div class="room-icon">🟣</div>

      <h3>روم الأسئلة</h3>

      <p>
        اطرح سؤالك وناقشه مع الطلاب.
      </p>

      <span>👥 120 طالب</span>

      <button onclick="joinRoom('روم الأسئلة')">
        دخول الروم
      </button>
    </div>

  </div>

</section>


<section id="tests" class="section alt-section">

  <div class="section-title">
    <div>
      <span>اختبر معلوماتك</span>
      <h2>📝 الاختبارات</h2>
    </div>
  </div>


  <div class="test-card">

    <div>
      <span class="tag">اختبار تجريبي</span>

      <h3>اختبار الوحدة الأولى</h3>

      <p>
        20 سؤالًا • 30 دقيقة • مستوى متوسط
      </p>
    </div>

    <button class="primary-btn" onclick="startTest()">
      ابدأ الاختبار 🚀
    </button>

  </div>

</section>


<section id="teacher" class="section teacher-section">

  <div class="teacher-box">

    <div class="teacher-avatar">
      👨‍🏫
    </div>

    <div>

      <span>مدرس الرياضيات</span>

      <h2>الأستاذ</h2>

      <p>
        شرح مبسط، متابعة، مراجعة واستعداد شامل لامتحانات التوجيهي.
      </p>

      <div class="teacher-contact">
        📞 <strong>رقم الأستاذ:</strong>
        <span>ضع الرقم هنا</span>
      </div>

      <button class="primary-btn" onclick="contactTeacher()">
        تواصل مع الأستاذ
      </button>

    </div>

  </div>

</section>


<section class="cta">

  <h2>جاهز تبدأ؟ 🚀</h2>

  <p>
    اجعل الرياضيات أسهل مع منبر ون.
  </p>

  <button onclick="scrollToSection('lessons')">
    ابدأ التعلم الآن
  </button>

</section>

</main>


<footer>

  <div class="footer-logo">
    <strong>منبر ون</strong>
    <span>MINBAR ONE</span>
  </div>

  <p>
    منصة تعليمية لطلاب التوجيهي والرياضيات.
  </p>

  <div class="footer-links">
    <a href="#home">الرئيسية</a>
    <a href="#lessons">الحصص</a>
    <a href="#summaries">الملخصات</a>
    <a href="#tests">الاختبارات</a>
  </div>

  <small>
    © 2026 منبر ون — جميع الحقوق محفوظة
  </small>

</footer>


<div id="modal" class="modal">

  <div class="modal-content">

    <button class="close-btn" onclick="closeModal()">×</button>

    <div id="modalContent"></div>

  </div>

</div>


<script src="script.js"></script>

</body>
</html>
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

html {
  scroll-behavior: smooth;
}

body {
  font-family: Arial, Tahoma, sans-serif;
  background: #f7f9fc;
  color: #172033;
  line-height: 1.7;
}

button,
input {
  font-family: inherit;
}

button {
  cursor: pointer;
  border: none;
}

.navbar {
  position: sticky;
  top: 0;
  z-index: 1000;

  display: flex;
  align-items: center;
  justify-content: space-between;

  padding: 15px 6%;

  background: rgba(255,255,255,.95);
  backdrop-filter: blur(12px);

  border-bottom: 1px solid #e6eaf0;
}

.logo {
  display: flex;
  align-items: center;
  gap: 10px;
}

.logo strong {
  display: block;
  font-size: 22px;
}

.logo small {
  display: block;
  font-size: 9px;
  letter-spacing: 2px;
  color: #64748b;
}

.logo-icon {
  width: 44px;
  height: 44px;

  display: grid;
  place-items: center;

  border-radius: 12px;

  background: #172033;
  color: white;

  font-size: 25px;
  font-weight: bold;
}

nav {
  display: flex;
  gap: 22px;
}

nav a {
  text-decoration: none;
  color: #475569;
  font-size: 14px;
}

nav a:hover {
  color: #172033;
}

.nav-actions {
  display: flex;
  gap: 8px;
}

.icon-btn,
.login-btn {
  padding: 10px 14px;
  border-radius: 10px;
}

.icon-btn {
  background: #eef2f7;
}

.login-btn {
  background: #172033;
  color: white;
}

.hero {
  min-height: 650px;

  display: flex;
  align-items: center;
  justify-content: space-between;

  gap: 50px;
  padding: 80px 8%;

  background:
    radial-gradient(circle at 20% 20%, #e6edff, transparent 30%),
    linear-gradient(135deg, #ffffff, #f2f5fa);
}

.hero-content {
  max-width: 650px;
}

.badge,
.tag {
  display: inline-block;

  padding: 6px 12px;

  border-radius: 30px;

  background: #e9eef8;
  color: #40516f;

  font-size: 12px;
}

.hero h1 {
  margin: 20px 0;

  font-size: clamp(40px, 6vw, 72px);
  line-height: 1.15;
}

.hero h1 span {
  display: block;
}

.hero p {
  color: #64748b;
  font-size: 18px;
  max-width: 560px;
}

.hero-buttons {
  display: flex;
  gap: 12px;
  margin-top: 30px;
}

.primary-btn,
.secondary-btn {
  padding: 13px 22px;
  border-radius: 12px;
  font-weight: bold;
}

.primary-btn {
  background: #172033;
  color: white;
}

.secondary-btn {
  background: white;
  border: 1px solid #dce2eb;
  color: #172033;
}

.hero-stats {
  display: flex;
  gap: 40px;
  margin-top: 50px;
}

.hero-stats strong,
.hero-stats span {
  display: block;
}

.hero-stats strong {
  font-size: 26px;
}

.hero-stats span {
  color: #64748b;
  font-size: 12px;
}

.hero-card {
  width: 380px;
  height: 420px;

  display: grid;
  place-items: center;

  border-radius: 30px;

  background: #172033;

  box-shadow: 0 25px 70px rgba(23,32,51,.25);

  transform: rotate(2deg);
}

.math-display {
  text-align: center;
  color: white;
}

.math-display span {
  color: #b9c5dc;
}

.formula {
  margin: 30px 0;

  font-size: 32px;
  font-weight: bold;
}

.features {
  display: grid;
  grid-template-columns: repeat(4,1fr);
  gap: 18px;

  padding: 50px 8%;
}

.feature-card {
  padding: 25px;

  background: white;

  border: 1px solid #e8ecf2;
  border-radius: 18px;

  transition: .25s;
}

.feature-card:hover {
  transform: translateY(-5px);
}

.feature-card div {
  font-size: 32px;
}

.feature-card h3 {
  margin: 12px 0 5px;
}

.feature-card p {
  color: #64748b;
  font-size: 13px;
}

.section {
  padding: 80px 8%;
}

.alt-section {
  background: #eef2f7;
}

.section-title {
  display: flex;
  justify-content: space-between;
  align-items: end;

  margin-bottom: 30px;
}

.section-title span {
  color: #64748b;
  font-size: 13px;
}

.section-title h2 {
  font-size: 32px;
}

#lessonSearch {
  width: 260px;

  padding: 13px 16px;

  border: 1px solid #dce2eb;
  border-radius: 12px;

  outline: none;
}

.filter-buttons {
  display: flex;
  gap: 8px;
  margin-bottom: 25px;
}

.filter-buttons button {
  padding: 8px 15px;

  border-radius: 9px;

  background: white;
  border: 1px solid #dde3eb;
}

.cards {
  display: grid;
  grid-template-columns: repeat(4,1fr);
  gap: 20px;
}

.lesson-card,
.summary-card {
  overflow: hidden;

  background: white;

  border: 1px solid #e4e9f0;
  border-radius: 18px;

  transition: .25s;
}

.lesson-card:hover,
.summary-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 15px 35px rgba(20,30,50,.08);
}

.video-placeholder {
  height: 180px;

  display: grid;
  place-items: center;

  background: #dce4f1;

  font-size: 45px;
  color: #172033;
}

.card-body {
  padding: 20px;
}

.card-body h3 {
  margin: 10px 0 5px;
}

.card-body p,
.summary-card p {
  color: #64748b;
  font-size: 13px;
}

.card-footer {
  display: flex;
  justify-content: space-between;
  align-items: center;

  margin-top: 20px;

  font-size: 12px;
  color: #64748b;
}

.card-footer button,
.summary-card button,
.room-card button {
  padding: 9px 14px;

  border-radius: 9px;

  background: #172033;
  color: white;
}

.summary-card {
  padding: 25px;
}

.file-icon {
  width: 55px;
  height: 65px;

  display: grid;
  place-items: center;

  border-radius: 10px;

  background: #e9eef8;

  font-weight: bold;
  font-size: 13px;
}

.summary-card h3 {
  margin: 15px 0 5px;
}

.summary-card button {
  margin-top: 20px;
}

.rooms-grid {
  display: grid;
  grid-template-columns: repeat(3,1fr);
  gap: 20px;
}

.room-card {
  padding: 28px;

  background: white;

  border: 1px solid #e4e9f0;
  border-radius: 20px;
}

.room-icon {
  font-size: 30px;
}

.room-card h3 {
  margin: 12px 0 5px;
}

.room-card p {
  color: #64748b;
  font-size: 14px;
}

.room-card span {
  display: block;

  margin: 18px 0;

  color: #64748b;
  font-size: 12px;
}

.test-card {
  display: flex;
  align-items: center;
  justify-content: space-between;

  padding: 35px;

  background: white;

  border-radius: 20px;
  border: 1px solid #e3e8ef;
}

.teacher-section {
  background: #172033;
  color: white;
}

.teacher-box {
  max-width: 900px;
  margin: auto;

  display: flex;
  align-items: center;
  gap: 35px;
}

.teacher-avatar {
  min-width: 150px;
  height: 150px;

  display: grid;
  place-items: center;

  border-radius: 50%;

  background: #33415d;

  font-size: 60px;
}

.teacher-box p {
  color: #c4ccda;
  margin: 10px 0 20px;
}

.teacher-contact {
  margin-bottom: 20px;
}

.cta {
  text-align: center;
  padding: 80px 20px;
}

.cta h2 {
  font-size: 40px;
}

.cta p {
  color: #64748b;
  margin: 10px 0 25px;
}

.cta button {
  padding: 14px 25px;

  border-radius: 12px;

  background: #172033;
  color: white;
  font-weight: bold;
}

footer {
  padding: 45px 8%;

  background: #101827;
  color: white;

  text-align: center;
}

.footer-logo strong {
  display: block;
  font-size: 25px;
}

.footer-logo span {
  color: #9ba8be;
  font-size: 10px;
  letter-spacing: 2px;
}

footer p {
  color: #9ba8be;
  margin: 10px 0 20px;
}

.footer-links {
  display: flex;
  justify-content: center;
  gap: 20px;

  margin-bottom: 25px;
}

.footer-links a {
  color: white;
  text-decoration: none;
  font-size: 13px;
}

footer small {
  color: #748197;
}

.modal {
  position: fixed;
  inset: 0;

  display: none;
  align-items: center;
  justify-content: center;

  z-index: 2000;

  background: rgba(0,0,0,.6);
}

.modal.show {
  display: flex;
}

.modal-content {
  width: min(500px,90%);

  padding: 30px;

  background: white;

  border-radius: 20px;

  position: relative;
}

.close-btn {
  position: absolute;
  top: 10px;
  left: 15px;

  background: transparent;

  font-size: 25px;
}

.login-form input {
  width: 100%;

  padding: 13px;

  margin: 8px 0;

  border: 1px solid #dce2eb;
  border-radius: 10px;
}

.login-form button {
  width: 100%;

  padding: 13px;

  margin-top: 10px;

  border-radius: 10px;

  background: #172033;
  color: white;
}

body.dark {
  background: #0c1220;
  color: #eef2f8;
}

body.dark .navbar,
body.dark .lesson-card,
body.dark .summary-card,
body.dark .room-card,
body.dark .test-card,
body.dark .feature-card,
body.dark .modal-content {
  background: #151e30;
  border-color: #28344a;
}

body.dark .hero {
  background: #0c1220;
}

body.dark .alt-section {
  background: #101827;
}

body.dark nav a,
body.dark .hero p,
body.dark .feature-card p,
body.dark .card-body p,
body.dark .summary-card p,
body.dark .room-card p,
body.dark .room-card span,
body.dark .hero-stats span {
  color: #aab5c8;
}

body.dark #lessonSearch {
  background: #151e30;
  color: white;
}

@media(max-width:1000px) {

  nav {
    display: none;
  }

  .hero-card {
    width: 300px;
  }

  .features,
  .cards {
    grid-template-columns: repeat(2,1fr);
  }

  .rooms-grid {
    grid-template-columns: 1fr;
  }
}

@media(max-width:700px) {

  .navbar {
    padding: 12px 4%;
  }

  .hero {
    flex-direction: column;
    text-align: center;
    padding: 60px 5%;
  }

  .hero-card {
    width: 90%;
    height: 300px;
  }

  .hero-buttons,
  .hero-stats {
    justify-content: center;
  }

  .hero-stats {
    gap: 20px;
  }

  .features,
  .cards {
    grid-template-columns: 1fr;
  }

  .section-title {
    align-items: stretch;
    flex-direction: column;
    gap: 15px;
  }

  #lessonSearch {
    width: 100%;
  }

  .test-card {
    flex-direction: column;
    align-items: flex-start;
    gap: 25px;
  }

  .teacher-box {
    flex-direction: column;
    text-align: center;
  }

  .nav-actions .login-btn {
    display: none;
  }
}
function scrollToSection(id) {
  document.getElementById(id).scrollIntoView({
    behavior: "smooth"
  });
}


function toggleDarkMode() {
  document.body.classList.toggle("dark");

  const dark = document.body.classList.contains("dark");

  localStorage.setItem("darkMode", dark ? "on" : "off");
}


if (localStorage.getItem("darkMode") === "on") {
  document.body.classList.add("dark");
}


function openModal(html) {
  document.getElementById("modalContent").innerHTML = html;
  document.getElementById("modal").classList.add("show");
}


function closeModal() {
  document.getElementById("modal").classList.remove("show");
}


function openLogin() {

  openModal(`
    <h2>👋 أهلاً بك في منبر ون</h2>

    <p style="color:#64748b;margin:10px 0 20px">
      سجل دخولك لمتابعة رحلتك التعليمية.
    </p>

    <div class="login-form">

      <input
        type="text"
        placeholder="رقم الهاتف أو البريد الإلكتروني"
      >

      <input
        type="password"
        placeholder="كلمة المرور"
      >

      <button onclick="loginDemo()">
        تسجيل الدخول
      </button>

    </div>
  `);
}


function loginDemo() {

  closeModal();

  setTimeout(() => {

    openModal(`
      <div style="text-align:center">

        <div style="font-size:50px">🎉</div>

        <h2>مرحبًا بك في منبر ون!</h2>

        <p style="color:#64748b">
          هذه نسخة تجريبية من حساب الطالب.
        </p>

        <div style="
          margin-top:20px;
          padding:20px;
          background:#eef2f7;
          border-radius:15px;
        ">

          <strong>📊 تقدمك</strong>

          <p>68% من الخطة التعليمية</p>

          <p>🔥 7 أيام متتالية</p>

          <p>⭐ 1,240 نقطة</p>

        </div>

      </div>
    `);

  }, 200);
}


function playLesson(title) {

  openModal(`

    <h2>🎥 ${title}</h2>

    <div style="
      height:250px;
      margin-top:20px;
      display:grid;
      place-items:center;
      background:#172033;
      color:white;
      border-radius:15px;
      font-size:50px;
    ">
      ▶
    </div>

    <p style="margin-top:15px;color:#64748b">
      هنا سيتم وضع فيديو الحصة الحقيقي.
      يمكنك لاحقًا ربطه بيوتيوب أو ملف فيديو.
    </p>

  `);
}


function openFile(title) {

  openModal(`

    <h2>📄 ${title}</h2>

    <p style="margin:20px 0;color:#64748b">
      هنا سيتم فتح ملف الـ PDF الحقيقي.
    </p>

    <button
      class="primary-btn"
      onclick="closeModal()"
    >
      إغلاق
    </button>

  `);
}


function joinRoom(room) {

  openModal(`

    <div style="text-align:center">

      <div style="font-size:50px">💬</div>

      <h2>${room}</h2>

      <p style="color:#64748b">
        الروم جاهز للربط بنظام المحادثة الحقيقي.
      </p>

      <button
        class="primary-btn"
        onclick="closeModal()"
      >
        متابعة
      </button>

    </div>

  `);
}


function startTest() {

  openModal(`

    <h2>📝 اختبار الوحدة الأولى</h2>

    <p style="color:#64748b;margin:15px 0">
      هذا نموذج تجريبي. سيتم لاحقًا إضافة بنك الأسئلة
      والتصحيح والنتائج.
    </p>

    <div style="
      padding:20px;
      background:#eef2f7;
      border-radius:15px;
    ">

      <strong>السؤال 1</strong>

      <p style="margin:10px 0">
        إذا كان x + 5 = 10 فما قيمة x؟
      </p>

      <button
        onclick="answerTest(5)"
        style="display:block;width:100%;padding:10px;margin:6px 0;border-radius:8px"
      >
        5
      </button>

      <button
        onclick="answerTest(10)"
        style="display:block;width:100%;padding:10px;margin:6px 0;border-radius:8px"
      >
        10
      </button>

      <button
        onclick="answerTest(15)"
        style="display:block;width:100%;padding:10px;margin:6px 0;border-radius:8px"
      >
        15
      </button>

    </div>

  `);
}


function answerTest(answer) {

  if (answer === 5) {

    openModal(`
      <div style="text-align:center">
        <div style="font-size:55px">✅</div>
        <h2>إجابة صحيحة!</h2>
        <p>أحسنت 👏</p>
      </div>
    `);

  } else {

    openModal(`
      <div style="text-align:center">
        <div style="font-size:55px">❌</div>
        <h2>ليست الإجابة الصحيحة</h2>
        <p>حاول مرة أخرى وتذكر أن:</p>
        <strong>x = 10 - 5 = 5</strong>
      </div>
    `);

  }
}


function contactTeacher() {

  openModal(`

    <div style="text-align:center">

      <div style="font-size:50px">👨‍🏫</div>

      <h2>التواصل مع الأستاذ</h2>

      <p style="color:#64748b;margin:15px">
        ضع رقم الأستاذ الحقيقي في ملف
        <strong>index.html</strong>.
      </p>

      <button
        class="primary-btn"
        onclick="closeModal()"
      >
        إغلاق
      </button>

    </div>

  `);
}


function filterLessons(unit) {

  const cards =
    document.querySelectorAll(".lesson-card");

  cards.forEach(card => {

    if (
      unit === "all" ||
      card.dataset.unit === unit
    ) {

      card.style.display = "";

    } else {

      card.style.display = "none";

    }

  });

}


function searchLessons() {

  const query =
    document.getElementById("lessonSearch")
    .value
    .toLowerCase();

  const cards =
    document.querySelectorAll(".lesson-card");

  cards.forEach(card => {

    const text =
      card.innerText.toLowerCase();

    card.style.display =
      text.includes(query)
      ? ""
      : "none";

  });

}


window.onclick = function(event) {

  const modal =
    document.getElementById("modal");

  if (event.target === modal) {
    closeModal();
  }

};
