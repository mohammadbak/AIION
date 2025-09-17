<!DOCTYPE html>
<html lang="fa">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>BnbAI</title>
  <link href="https://fonts.googleapis.com/css2?family=Vazirmatn:wght@400;700&display=swap" rel="stylesheet">
  <style>
    /* Reset و فونت */
    * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Vazirmatn', sans-serif; scroll-behavior: smooth;}
    body { background: #f5f7fa; color: #333; line-height: 1.6;}
    a { text-decoration: none; color: inherit; }
    button { cursor: pointer; }

    /* هدر */
    header { background: linear-gradient(90deg, #6a11cb, #2575fc); color: white; padding: 20px 0; position: sticky; top: 0; z-index: 1000; }
    header .container { display: flex; justify-content: space-between; align-items: center; width: 90%; margin: auto; }
    header h1 { font-size: 1.8rem; }
    nav a { margin-left: 20px; font-weight: 500; transition: 0.3s; }
    nav a:hover { color: #ffd700; }

    /* بخش قهرمانی */
    .hero { display: flex; flex-direction: column; justify-content: center; align-items: center; text-align: center; padding: 120px 20px; background: #fff; }
    .hero h2 { font-size: 2.5rem; margin-bottom: 20px; color: #2575fc; animation: fadeInDown 1s ease forwards; }
    .hero p { font-size: 1.2rem; margin-bottom: 30px; max-width: 600px; animation: fadeInUp 1s ease forwards; }
    .hero button { padding: 15px 30px; background: #6a11cb; border: none; border-radius: 30px; color: white; font-weight: bold; transition: 0.3s; }
    .hero button:hover { background: #2575fc; }

    /* ویژگی‌ها */
    .features { display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 30px; width: 90%; margin: 60px auto; }
    .feature { background: white; padding: 30px; border-radius: 20px; box-shadow: 0 10px 25px rgba(0,0,0,0.1); text-align: center; transition: 0.3s; }
    .feature:hover { transform: translateY(-10px); }
    .feature h3 { margin-bottom: 15px; color: #6a11cb; }
    .feature p { color: #555; }

    /* فرم تماس */
    .contact { background: #2575fc; color: white; padding: 80px 20px; text-align: center; }
    .contact h2 { margin-bottom: 30px; }
    .contact form { display: flex; flex-direction: column; max-width: 500px; margin: auto; }
    .contact input, .contact textarea { padding: 15px; margin-bottom: 20px; border: none; border-radius: 10px; font-size: 1rem; }
    .contact button { padding: 15px; border: none; border-radius: 30px; background: #6a11cb; color: white; font-weight: bold; transition: 0.3s; }
    .contact button:hover { background: #fff; color: #2575fc; }

    /* فوتر */
    footer { text-align: center; padding: 30px 0; background: #1a1a1a; color: white; }

    /* انیمیشن‌ها */
    @keyframes fadeInDown { 0% { opacity: 0; transform: translateY(-30px);} 100% { opacity: 1; transform: translateY(0);} }
    @keyframes fadeInUp { 0% { opacity: 0; transform: translateY(30px);} 100% { opacity: 1; transform: translateY(0);} }
  </style>
</head>
<body>

  <header>
    <div class="container">
      <h1>BnbAI</h1>
      <nav>
        <a href="#features">ویژگی‌ها</a>
        <a href="#contact">تماس با ما</a>
      </nav>
    </div>
  </header>

  <section class="hero">
    <h2>هوش مصنوعی برای تجربه‌ای بهتر در سفر</h2>
    <p>BnbAI تجربه‌ای نوین از رزرو و مدیریت اقامتگاه‌ها با کمک هوش مصنوعی ارائه می‌دهد.</p>
    <button>شروع کنید</button>
  </section>

  <section class="features" id="features">
    <div class="feature">
      <h3>جستجوی هوشمند</h3>
      <p>با الگوریتم‌های پیشرفته ما بهترین گزینه‌های اقامتی را پیدا کنید.</p>
    </div>
    <div class="feature">
      <h3>قیمت بهینه</h3>
      <p>پیشنهادات ویژه و تخفیف‌های هوشمند برای سفرهای شما.</p>
    </div>
    <div class="feature">
      <h3>پشتیبانی ۲۴/۷</h3>
      <p>تیم ما همیشه آماده پاسخگویی به سوالات و مشکلات شماست.</p>
    </div>
  </section>

  <section class="contact" id="contact">
    <h2>تماس با ما</h2>
    <form>
      <input type="text" placeholder="نام شما" required>
      <input type="email" placeholder="ایمیل شما" required>
      <textarea rows="5" placeholder="پیام شما" required></textarea>
      <button type="submit">ارسال پیام</button>
    </form>
  </section>

  <footer>
    &copy; 2025 BnbAI. تمامی حقوق محفوظ است.
  </footer>

</body>
</html>
