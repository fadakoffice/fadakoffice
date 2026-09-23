<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
  <meta charset="UTF-8">

  <meta name="viewport"
        content="width=device-width, initial-scale=1.0">

  <meta name="description"
        content="دفتر خدمات کامپیوتری فدک - ارائه انواع خدمات کامپیوتری، اینترنتی، چاپ و خدمات اداری">

  <meta name="theme-color" content="#2563eb">

  <title>دفتر خدمات کامپیوتری فدک</title>

  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    html {
      scroll-behavior: smooth;
    }

    body {
      font-family:
        Tahoma,
        Arial,
        sans-serif;
      background: #f5f7fb;
      color: #1f2937;
      line-height: 1.9;
    }

    a {
      text-decoration: none;
      color: inherit;
    }

    /* ===== Header ===== */

    header {
      background: linear-gradient(135deg, #1d4ed8, #2563eb);
      color: white;
      position: sticky;
      top: 0;
      z-index: 1000;
      box-shadow: 0 3px 15px rgba(0,0,0,0.15);
    }

    .header-inner {
      max-width: 1150px;
      margin: auto;
      padding: 14px 20px;
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 20px;
    }

    .logo {
      display: flex;
      align-items: center;
      gap: 12px;
    }

    .logo-icon {
      width: 48px;
      height: 48px;
      border-radius: 14px;
      background: white;
      color: #2563eb;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 25px;
      font-weight: bold;
    }

    .logo-text h1 {
      font-size: 19px;
      margin-bottom: 0;
    }

    .logo-text span {
      font-size: 12px;
      opacity: 0.9;
    }

    nav {
      display: flex;
      gap: 8px;
      flex-wrap: wrap;
    }

    nav a {
      padding: 7px 12px;
      border-radius: 8px;
      font-size: 14px;
      transition: 0.2s;
    }

    nav a:hover {
      background: rgba(255,255,255,0.18);
    }

    /* ===== Hero ===== */

    .hero {
      background:
        linear-gradient(
          135deg,
          rgba(30,64,175,0.95),
          rgba(37,99,235,0.9)
        );
      color: white;
      padding: 85px 20px;
      text-align: center;
    }

    .hero-content {
      max-width: 850px;
      margin: auto;
    }

    .hero h2 {
      font-size: 38px;
      margin-bottom: 18px;
    }

    .hero p {
      font-size: 18px;
      opacity: 0.95;
      margin-bottom: 28px;
    }

    .hero-buttons {
      display: flex;
      justify-content: center;
      gap: 12px;
      flex-wrap: wrap;
    }

    .btn {
      display: inline-block;
      padding: 12px 25px;
      border-radius: 10px;
      font-weight: bold;
      transition: 0.25s;
    }

    .btn-primary {
      background: white;
      color: #1d4ed8;
    }

    .btn-primary:hover {
      transform: translateY(-2px);
    }

    .btn-outline {
      border: 2px solid white;
      color: white;
    }

    .btn-outline:hover {
      background: white;
      color: #1d4ed8;
    }

    /* ===== General ===== */

    .container {
      max-width: 1150px;
      margin: auto;
      padding: 65px 20px;
    }

    .section-title {
      text-align: center;
      margin-bottom: 40px;
    }

    .section-title h2 {
      color: #1d4ed8;
      font-size: 30px;
      margin-bottom: 8px;
    }

    .section-title p {
      color: #6b7280;
    }

    /* ===== Services ===== */

    .services {
      display: grid;
      grid-template-columns:
        repeat(auto-fit, minmax(220px, 1fr));
      gap: 20px;
    }

    .service-card {
      background: white;
      padding: 28px 22px;
      border-radius: 16px;
      text-align: center;
      box-shadow: 0 5px 20px rgba(0,0,0,0.07);
      border: 1px solid #e5e7eb;
      transition: 0.25s;
    }

    .service-card:hover {
      transform: translateY(-5px);
      box-shadow: 0 10px 25px rgba(0,0,0,0.12);
    }

    .service-icon {
      width: 65px;
      height: 65px;
      margin: 0 auto 15px;
      border-radius: 50%;
      background: #eff6ff;
      color: #2563eb;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 30px;
    }

    .service-card h3 {
      margin-bottom: 8px;
      color: #111827;
    }

    .service-card p {
      color: #6b7280;
      font-size: 14px;
    }

    /* ===== About ===== */

    .about {
      background: white;
    }

    .about-box {
      max-width: 850px;
      margin: auto;
      background: #f8fafc;
      padding: 30px;
      border-radius: 18px;
      border-right: 5px solid #2563eb;
    }

    .about-box p {
      margin-bottom: 12px;
    }

    .features {
      margin-top: 20px;
      display: grid;
      grid-template-columns:
        repeat(auto-fit, minmax(180px, 1fr));
      gap: 12px;
    }

    .feature {
      background: white;
      padding: 13px;
      border-radius: 10px;
      border: 1px solid #e5e7eb;
    }

    /* ===== Contact ===== */

    .contact-section {
      background: #eef4ff;
    }

    .contact-grid {
      display: grid;
      grid-template-columns:
        repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
    }

    .contact-card {
      background: white;
      padding: 25px;
      border-radius: 16px;
      text-align: center;
      box-shadow: 0 5px 18px rgba(0,0,0,0.06);
    }

    .contact-card .icon {
      font-size: 32px;
      margin-bottom: 10px;
    }

    .contact-card h3 {
      color: #1d4ed8;
      margin-bottom: 8px;
    }

    .contact-card p {
      color: #555;
    }

    /* ===== CTA ===== */

    .cta {
      margin-top: 45px;
      background: linear-gradient(135deg, #1d4ed8, #2563eb);
      color: white;
      border-radius: 20px;
      padding: 40px 25px;
      text-align: center;
    }

    .cta h2 {
      margin-bottom: 12px;
    }

    .cta p {
      margin-bottom: 20px;
      opacity: 0.95;
    }

    /* ===== Footer ===== */

    footer {
      background: #111827;
      color: white;
      text-align: center;
      padding: 30px 20px;
    }

    footer p {
      margin: 5px 0;
      color: #d1d5db;
      font-size: 14px;
    }

    .footer-name {
      color: white;
      font-size: 18px;
      font-weight: bold;
    }

    /* ===== Mobile ===== */

    @media (max-width: 700px) {

      .header-inner {
        flex-direction: column;
        gap: 8px;
      }

      nav {
        justify-content: center;
      }

      nav a {
        font-size: 13px;
        padding: 5px 8px;
      }

      .hero {
        padding: 60px 18px;
      }

      .hero h2 {
        font-size: 28px;
      }

      .hero p {
        font-size: 16px;
      }

      .container {
        padding: 50px 16px;
      }

      .section-title h2 {
        font-size: 25px;
      }
    }
  </style>
</head>

<body>

  <!-- ===== Header ===== -->

  <header>
    <div class="header-inner">

      <div class="logo">
        <div class="logo-icon">ف</div>

        <div class="logo-text">
          <h1>دفتر خدمات کامپیوتری فدک</h1>
          <span>خدمات کامپیوتری و اینترنتی</span>
        </div>
      </div>

      <nav>
        <a href="#home">خانه</a>
        <a href="#services">خدمات</a>
        <a href="#about">درباره ما</a>
        <a href="#contact">تماس با ما</a>
      </nav>

    </div>
  </header>


  <!-- ===== Hero ===== -->

  <section class="hero" id="home">

    <div class="hero-content">

      <h2>دفتر خدمات کامپیوتری فدک</h2>

      <p>
        ارائه خدمات کامپیوتری، اینترنتی، چاپ،
        ثبت‌نام‌های اینترنتی و خدمات اداری
      </p>

      <div class="hero-buttons">

        <a class="btn btn-primary"
           href="#services">
          مشاهده خدمات
        </a>

        <a class="btn btn-outline"
           href="#contact">
          تماس با ما
        </a>

      </div>

    </div>

  </section>


  <!-- ===== Services ===== -->

  <section id="services">

    <div class="container">

      <div class="section-title">

        <h2>خدمات ما</h2>

        <p>
          بخشی از خدمات ارائه‌شده در دفتر خدمات کامپیوتری فدک
        </p>

      </div>


      <div class="services">

        <div class="service-card">

          <div class="service-icon">💻</div>

          <h3>خدمات کامپیوتری</h3>

          <p>
            تایپ، ویرایش، تنظیم و آماده‌سازی
            انواع فایل‌های کامپیوتری
          </p>

        </div>


        <div class="service-card">

          <div class="service-icon">🖨️</div>

          <h3>چاپ و کپی</h3>

          <p>
            چاپ و کپی اسناد و مدارک
            با کیفیت مناسب
          </p>

        </div>


        <div class="service-card">

          <div class="service-icon">🌐</div>

          <h3>خدمات اینترنتی</h3>

          <p>
            انجام امور اینترنتی و
            ثبت‌نام‌های آنلاین
          </p>

        </div>


        <div class="service-card">

          <div class="service-icon">📄</div>

          <h3>خدمات اداری</h3>

          <p>
            آماده‌سازی فرم‌ها،
            مدارک و امور اداری
          </p>

        </div>


        <div class="service-card">

          <div class="service-icon">📝</div>

          <h3>تایپ و ویرایش</h3>

          <p>
            تایپ فارسی و انگلیسی،
            ویرایش و صفحه‌آرایی
          </p>

        </div>


        <div class="service-card">

          <div class="service-icon">📑</div>

          <h3>اسکن مدارک</h3>

          <p>
            اسکن و آماده‌سازی
            مدارک و اسناد
          </p>

        </div>


        <div class="service-card">

          <div class="service-icon">📧</div>

          <h3>خدمات ایمیل</h3>

          <p>
            ایجاد و مدیریت ایمیل
            و انجام امور مرتبط
          </p>

        </div>


        <div class="service-card">

          <div class="service-icon">🖥️</div>

          <h3>خدمات نرم‌افزاری</h3>

          <p>
            نصب و تنظیم نرم‌افزارها
            و خدمات مرتبط با رایانه
          </p>

        </div>

      </div>

    </div>

  </section>


  <!-- ===== About ===== -->

  <section class="about" id="about">

    <div class="container">

      <div class="section-title">

        <h2>درباره دفتر فدک</h2>

        <p>
          همراه شما در انجام امور کامپیوتری و اینترنتی
        </p>

      </div>


      <div class="about-box">

        <p>
          <strong>دفتر خدمات کامپیوتری فدک</strong>
          با هدف ارائه خدمات کامپیوتری،
          اینترنتی و اداری فعالیت می‌کند.
        </p>

        <p>
          تلاش ما این است که خدمات مورد نیاز
          شما را با دقت، سرعت و کیفیت مناسب
          ارائه کنیم.
        </p>


        <div class="features">

          <div class="feature">
            ✅ انجام سریع خدمات
          </div>

          <div class="feature">
            ✅ خدمات متنوع
          </div>

          <div class="feature">
            ✅ پشتیبانی و راهنمایی
          </div>

          <div class="feature">
            ✅ محیط مناسب
          </div>

        </div>

      </div>

    </div>

  </section>


  <!-- ===== Contact ===== -->

  <section class="contact-section" id="contact">

    <div class="container">

      <div class="section-title">

        <h2>تماس با ما</h2>

        <p>
          برای دریافت اطلاعات بیشتر با دفتر فدک تماس بگیرید
        </p>

      </div>


      <div class="contact-grid">


        <div class="contact-card">

          <div class="icon">📍</div>

          <h3>آدرس</h3>

          <p>
            آدرس دفتر را اینجا وارد کنید
          </p>

        </div>


        <div class="contact-card">

          <div class="icon">📞</div>

          <h3>تلفن</h3>

          <p>
            شماره تماس را اینجا وارد کنید
          </p>

        </div>


        <div class="contact-card">

          <div class="icon">📱</div>

          <h3>موبایل</h3>

          <p>
            شماره موبایل را اینجا وارد کنید
          </p>

        </div>


        <div class="contact-card">

          <div class="icon">🕐</div>

          <h3>ساعات کاری</h3>

          <p>
            ساعات کاری را اینجا وارد کنید
          </p>

        </div>


      </div>


      <div class="cta">

        <h2>
          دفتر خدمات کامپیوتری فدک
        </h2>

        <p>
          آماده ارائه خدمات کامپیوتری و اینترنتی به شما هستیم.
        </p>

        <a class="btn btn-primary"
           href="#home">
          بازگشت به صفحه اصلی
        </a>

      </div>

    </div>

  </section>


  <!-- ===== Footer ===== -->

  <footer>

    <p class="footer-name">
      دفتر خدمات کامپیوتری فدک
    </p>

    <p>
      خدمات کامپیوتری، اینترنتی و اداری
    </p>

    <p>
      © ۱۴۰۵ - تمامی حقوق محفوظ است.
    </p>

  </footer>


</body>
</html>
