# <!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>منبر ون | منصة الرياضيات</title>

  <style>
    * {
      box-sizing: border-box;
    }

    body {
      margin: 0;
      font-family: Arial, Tahoma, sans-serif;
      background: #f5f7fb;
      color: #172033;
    }

    header {
      background: #172033;
      color: white;
      padding: 18px 6%;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    .logo {
      font-size: 25px;
      font-weight: bold;
    }

    nav a {
      color: white;
      text-decoration: none;
      margin: 0 8px;
      font-size: 14px;
    }

    .hero {
      padding: 80px 8%;
      text-align: center;
      background: linear-gradient(135deg, #ffffff, #e9eef8);
    }

    .hero h1 {
      font-size: 48px;
      margin: 10px 0;
    }

    .hero h1 span {
      display: block;
    }

    .hero p {
      color: #64748b;
      font-size: 18px;
      max-width: 600px;
      margin: 20px auto;
    }

    button {
      border: none;
      background: #172033;
      color: white;
      padding: 13px 25px;
      border-radius: 10px;
      cursor: pointer;
      font-weight: bold;
    }

    .features {
      padding: 60px 8%;
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 20px;
    }

    .card {
      background: white;
      padding: 25px;
      border-radius: 18px;
      text-align: center;
      box-shadow: 0 5px 20px rgba(0,0,0,.06);
    }

    .card .icon {
      font-size: 38px;
    }

    .card p {
      color: #64748b;
      font-size: 14px;
    }

    .section {
      padding: 70px 8%;
    }

    .section h2 {
      font-size: 32px;
    }

    .lesson {
      background: white;
      padding: 25px;
      border-radius: 18px;
      margin-top: 20px;
    }

    footer {
      background: #101827;
      color: white;
      text-align: center;
      padding: 40px;
    }

    @media (max-width: 700px) {
      header {
        flex-direction: column;
        gap: 15px;
      }

      nav {
        text-align: center;
      }

      .hero h1 {
        font-size: 38px;
      }

      .features {
        grid-template-columns: 1fr 1fr;
        padding: 40px 5%;
      }

      .section {
        padding: 50px 5%;
      }
    }
  </style>
</head>

<body>

<header>
  <div class="logo">∑ منبر ون</div>

  <nav>
    <a href="#home">الرئيسية</a>
    <a href="#lessons">الحصص</a>
    <a href="#summaries">الملخصات</a>
    <a href="#rooms">الرومات</a>
    <a href="#tests">الاختبارات</a>
  </nav>
</header>

<section id="home" class="hero">

  <h1>
    الرياضيات أصبحت
    <span>أسهل مع منبر ون 🚀</span>
  </h1>

  <p>
    منصة تعليمية متخصصة لطلاب التوجيهي،
    تجمع الحصص والملخصات والاختبارات والرومات التعليمية في مكان واحد.
  </p>

  <button onclick="document.getElementById('lessons').scrollIntoView()">
    ابدأ التعلم
  </button>

</section>

<section class="features">

  <div class="card">
    <div class="icon">🎥</div>
    <h3>الحصص</h3>
    <p>حصص وفيديوهات تعليمية مرتبة.</p>
  </div>

  <div class="card">
    <div class="icon">📚</div>
    <h3>الملخصات</h3>
    <p>ملخصات وقوانين للمراجعة.</p>
  </div>

  <div class="card">
    <div class="icon">💬</div>
    <h3>الرومات</h3>
    <p>رومات للنقاش وطرح الأسئلة.</p>
  </div>

  <div class="card">
    <div class="icon">📝</div>
    <h3>الاختبارات</h3>
    <p>اختبارات تدريبية لقياس مستواك.</p>
  </div>

</section>

<section id="lessons" class="section">

  <h2>🎥 الحصص التعليمية</h2>

  <div class="lesson">
    <h3>الحصة الأولى</h3>
    <p>سيتم إضافة فيديو الحصة هنا.</p>
    <button>مشاهدة الحصة</button>
  </div>

  <div class="lesson">
    <h3>الحصة الثانية</h3>
    <p>سيتم إضافة فيديو الحصة هنا.</p>
    <button>مشاهدة الحصة</button>
  </div>

</section>

<section id="summaries" class="section">

  <h2>📚 الملخصات</h2>

  <div class="lesson">
    <h3>ملخص الوحدة الأولى</h3>
    <p>سيتم إضافة ملف PDF هنا.</p>
    <button>فتح الملخص</button>
  </div>

</section>

<section id="rooms" class="section">

  <h2>💬 الرومات التعليمية</h2>

  <div class="lesson">
    <h3>روم الرياضيات العام</h3>
    <p>مكان لمناقشة الأسئلة والاستفسارات.</p>
    <button>دخول الروم</button>
  </div>

</section>

<section id="tests" class="section">

  <h2>📝 الاختبارات</h2>

  <div class="lesson">
    <h3>اختبار الوحدة الأولى</h3>
    <p>اختبار تجريبي لقياس مستواك.</p>
    <button>ابدأ الاختبار</button>
  </div>

</section>

<footer>

  <h2>منبر ون</h2>

  <p>
    منصة الرياضيات لطلاب التوجيهي
  </p>

  <p>
    © 2026 منبر ون
  </p>

</footer>

</body>
</html>
