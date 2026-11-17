# --7-4----
<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>AMIR SG | علوم هفتم</title>

<style>
@import url('https://fonts.googleapis.com/css2?family=Vazirmatn:wght@400;500;700;800;900&display=swap');

:root {
  --blue: #087cf0;
  --cyan: #19c7d9;
  --dark: #071426;
  --panel: rgba(12, 30, 54, .88);
  --white: #f3f8ff;
}

* {
  box-sizing: border-box;
  scroll-behavior: smooth;
}

body {
  margin: 0;
  font-family: Vazirmatn, Tahoma, sans-serif;
  color: var(--white);
  background:
    radial-gradient(ellipse at 15% 15%, #123b68 0, transparent 38%),
    radial-gradient(ellipse at 85% 75%, #073b54 0, transparent 40%),
    linear-gradient(135deg, #06101f, #0b1c35 55%, #071426);
  min-height: 100vh;
  overflow-x: hidden;
}

/* پس‌زمینه اختصاصی با نام امیرحسین مواظب */
body::before {
  content: "امیرحسین مواظب  •  AMIR SG  •  امیرحسین مواظب  •  AMIR SG  •  امیرحسین مواظب  •  AMIR SG  •  امیرحسین مواظب  •  AMIR SG  •  امیرحسین مواظب  •  AMIR SG";
  position: fixed;
  inset: -100px;
  z-index: -1;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  font-size: clamp(22px, 4vw, 48px);
  font-weight: 900;
  line-height: 3.2;
  letter-spacing: 8px;
  color: rgba(83, 181, 255, .10);
  transform: rotate(-20deg) scale(1.3);
  pointer-events: none;
  word-spacing: 25px;
}

header {
  padding: 24px 6%;
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap;
  gap: 15px;
  background: rgba(3, 13, 27, .8);
  border-bottom: 1px solid rgba(62, 176, 255, .25);
  backdrop-filter: blur(12px);
}

.logo {
  font-size: 27px;
  font-weight: 900;
  color: #fff;
  letter-spacing: 2px;
}

.logo span {
  color: var(--cyan);
}

nav {
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
}

nav a {
  text-decoration: none;
  color: #d9ecff;
  padding: 9px 14px;
  border-radius: 10px;
  transition: .2s;
}

nav a:hover {
  background: var(--blue);
  color: white;
}

.hero {
  text-align: center;
  padding: 75px 20px 55px;
}

.hero small {
  color: var(--cyan);
  font-weight: 700;
  letter-spacing: 2px;
}

.hero h1 {
  font-size: clamp(32px, 6vw, 58px);
  margin: 18px 0;
  font-weight: 900;
}

.hero h1 span {
  color: var(--cyan);
}

.hero p {
  color: #c1d5ed;
  line-height: 2;
  max-width: 700px;
  margin: auto;
}

.container {
  width: min(1100px, 92%);
  margin: auto;
}

.section-title {
  font-size: 27px;
  margin: 35px 0 20px;
  border-right: 4px solid var(--cyan);
  padding-right: 14px;
}

.cards {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(230px, 1fr));
  gap: 18px;
}

.card, .lesson, .quiz-box {
  background: var(--panel);
  border: 1px solid rgba(77, 173, 255, .25);
  border-radius: 18px;
  padding: 22px;
  box-shadow: 0 12px 35px rgba(0,0,0,.18);
  backdrop-filter: blur(10px);
}

.card {
  transition: .25s;
}

.card:hover {
  transform: translateY(-6px);
  border-color: var(--cyan);
}

.card h3 {
  color: var(--cyan);
  margin-top: 0;
}

.card p, .lesson p, .lesson li {
  color: #d4e3f5;
  line-height: 2;
}

button {
  font-family: inherit;
  cursor: pointer;
  border: 0;
  border-radius: 10px;
  padding: 11px 18px;
  color: white;
  background: linear-gradient(110deg, #087cf0, #12b9d0);
  font-weight: 700;
  transition: .2s;
}

button:hover {
  filter: brightness(1.15);
  transform: translateY(-2px);
}

.lesson {
  margin: 18px 0;
  scroll-margin-top: 20px;
}

.lesson h2 {
  color: var(--cyan);
  margin-top: 0;
}

.lesson h3 {
  color: #8dc8ff;
}

.lesson ul {
  padding-right: 22px;
}

.answer {
  background: rgba(9, 125, 185, .13);
  border-right: 3px solid var(--cyan);
  padding: 12px 16px;
  border-radius: 9px;
  margin: 12px 0;
  line-height: 2;
}

.quiz-question {
  background: rgba(255,255,255,.04);
  padding: 15px;
  border-radius: 12px;
  margin: 14px 0;
}

.quiz-question label {
  display: block;
  padding: 7px;
  cursor: pointer;
  color: #dcecff;
}

#result {
  margin-top: 18px;
  font-size: 19px;
  color: var(--cyan);
  font-weight: 800;
}

footer {
  text-align: center;
  padding: 35px 15px;
  margin-top: 60px;
  background: rgba(2, 10, 22, .8);
  border-top: 1px solid rgba(62, 176, 255, .25);
  color: #b7cce2;
  line-height: 2.2;
}

footer strong {
  color: var(--cyan);
}

@media(max-width:600px) {
  header {
    justify-content: center;
  }
  nav {
    justify-content: center;
  }
  .hero {
    padding-top: 48px;
  }
}
</style>
</head>

<body>

<header>
  <div class="logo">AMIR <span>SG</span></div>
  <nav>
    <a href="#home">خانه</a>
    <a href="#lessons">درس‌ها</a>
    <a href="#quiz">آزمون</a>
  </nav>
</header>

<section class="hero" id="home">
  <small>AMIR SG EDUCATIONAL PROJECT</small>
  <h1>علوم تجربی <span>هفتم</span></h1>
  <p>
    یک محیط آموزشی برای یادگیری، مرور نکات مهم،
    مطالعه پرسش‌ها و سنجش آموخته‌ها
  </p>
  <p>تهیه و تنظیم: امیرحسین مواظب</p>
  <br>
  <a href="#lessons"><button>شروع یادگیری</button></a>
</section>

<main class="container">

<section id="lessons">
  <h2 class="section-title">فصل‌های آموزشی</h2>

  <div class="cards">
    <div class="card">
      <h3>درس پنجم</h3>
      <p>از معدن تا خانه</p>
      <a href="#lesson5"><button>مطالعه درس</button></a>
    </div>

    <div class="card">
      <h3>درس ششم</h3>
      <p>سفر آب روی زمین</p>
      <a href="#lesson6"><button>مطالعه درس</button></a>
    </div>

    <div class="card">
      <h3>درس هفتم</h3>
      <p>سفر آب درون زمین</p>
      <a href="#lesson7"><button>مطالعه درس</button></a>
    </div>
  </div>
</section>

<section class="lesson" id="lesson5">
  <h2>درس پنجم: از معدن تا خانه</h2>

  <h3>نکات مهم</h3>
  <ul>
    <li>مواد مورد نیاز زندگی انسان از منابع طبیعی به دست می‌آیند.</li>
    <li>بسیاری از فلزها از سنگ معدن استخراج می‌شوند.</li>
    <li>برای جدا کردن فلز از سنگ معدن، مراحل مختلفی انجام می‌شود.</li>
    <li>بازیافت فلزها باعث کاهش مصرف منابع طبیعی و انرژی می‌شود.</li>
    <li>استخراج بی‌رویه معادن می‌تواند به محیط زیست آسیب برساند.</li>
  </ul>

  <h3>واژه‌های مهم</h3>
  <div class="answer">
    <b>سنگ معدن:</b> سنگی که دارای مقدار مناسبی از یک ماده ارزشمند باشد.
  </div>
  <div class="answer">
    <b>بازیافت:</b> تبدیل مواد استفاده‌شده به مواد قابل استفاده دوباره.
  </div>

  <h3>پرسش و پاسخ</h3>
  <div class="answer">
    <b>۱. چرا فلزها را بازیافت می‌کنند؟</b><br>
    برای صرفه‌جویی در منابع طبیعی، انرژی و کاهش آلودگی محیط زیست.
  </div>
  <div class="answer">
    <b>۲. استخراج معدن چه تأثیری بر محیط زیست دارد؟</b><br>
    ممکن است باعث تخریب زیستگاه‌ها، آلودگی آب و خاک و تغییر شکل زمین شود.
  </div>
  <div class="answer">
    <b>۳. چرا مواد معدنی در زندگی اهمیت دارند؟</b><br>
    چون در ساخت وسایل، ساختمان‌ها، ابزارها و بسیاری از محصولات کاربرد دارند.
  </div>

  <h3>فعالیت و تحقیق</h3>
  <div class="answer">
    <b>نمونه پاسخ: چند وسیله فلزی در خانه نام ببرید.</b><br>
    قاشق، قابلمه، شیر آب، کلید و بدنه برخی وسایل برقی.
  </div>
  <div class="answer">
    <b>نمونه پاسخ: چگونه می‌توان مصرف منابع معدنی را کاهش داد؟</b><br>
    با استفاده درست از وسایل، تعمیر آن‌ها و بازیافت فلزها.
  </div>
  <p><b>پایان درس پنجم</b> | تهیه و تنظیم: امیرحسین مواظب</p>
</section>

<section class="lesson" id="lesson6">
  <h2>درس ششم: سفر آب روی زمین</h2>

  <h3>نکات مهم</h3>
  <ul>
    <li>بخش زیادی از سطح زمین را آب پوشانده است.</li>
    <li>آب در طبیعت به شکل‌های جامد، مایع و گاز وجود دارد.</li>
    <li>تبخیر، میعان، بارش و رواناب از مراحل چرخه آب هستند.</li>
    <li>خورشید انرژی لازم برای تبخیر آب را فراهم می‌کند.</li>
    <li>بخشی از آب باران و برف به رودخانه‌ها و دریاها می‌رسد.</li>
  </ul>

  <h3>واژه‌های مهم</h3>
  <div class="answer">
    <b>تبخیر:</b> تبدیل آب مایع به بخار آب.
  </div>
  <div class="answer">
    <b>میعان:</b> تبدیل بخار آب به قطره‌های ریز آب.
  </div>
  <div class="answer">
    <b>رواناب:</b> آبی که روی سطح زمین جاری می‌شود.
  </div>

  <h3>پرسش و پاسخ</h3>
  <div class="answer">
    <b>۱. چرخه آب چیست؟</b><br>
    گردش پیوسته آب بین سطح زمین، هوا و منابع آبی.
  </div>
  <div class="answer">
    <b>۲. عامل اصلی تبخیر آب در طبیعت چیست؟</b><br>
    انرژی گرمایی خورشید.
  </div>
  <div class="answer">
    <b>۳. ابرها چگونه تشکیل می‌شوند؟</b><br>
    بخار آب بالا می‌رود، سرد می‌شود و با میعان قطره‌های ریز آب یا بلورهای یخ تشکیل می‌دهد.
  </div>

  <h3>فعالیت و تحقیق</h3>
  <div class="answer">
    <b>نمونه پاسخ: چرا چرخه آب برای زندگی مهم است؟</b><br>
    چون باعث جابه‌جایی و تجدید آب در طبیعت می‌شود و آب مورد نیاز جانداران را فراهم می‌کند.
  </div>
  <div class="answer">
    <b>نمونه پاسخ: چند راه جلوگیری از هدررفت آب را بنویسید.</b><br>
    تعمیر نشتی شیرها، بستن شیر هنگام مسواک زدن و استفاده درست از آب.
  </div>
  <p><b>پایان درس ششم</b> | تهیه و تنظیم: امیرحسین مواظب</p>
</section>

<section class="lesson" id="lesson7">
  <h2>درس هفتم: سفر آب درون زمین</h2>

  <h3>نکات مهم</h3>
  <ul>
    <li>بخشی از آب باران و برف به درون زمین نفوذ می‌کند.</li>
    <li>آب‌های زیرزمینی در فضاهای خالی و شکاف سنگ‌ها جمع می‌شوند.</li>
    <li>آبخوان لایه یا مجموعه‌ای از لایه‌های زمین است که آب را در خود نگه می‌دارد و منتقل می‌کند.</li>
    <li>چاه‌ها برای دسترسی به آب زیرزمینی استفاده می‌شوند.</li>
    <li>برداشت بیش از اندازه آب زیرزمینی می‌تواند سطح آب را پایین ببرد.</li>
  </ul>

  <h3>واژه‌های مهم</h3>
  <div class="answer">
    <b>نفوذ:</b> وارد شدن آب به داخل خاک و زمین.
  </div>
  <div class="answer">
    <b>آبخوان:</b> لایه‌ای از زمین که می‌تواند آب زیرزمینی را ذخیره و منتقل کند.
  </div>
  <div class="answer">
    <b>سطح ایستابی:</b> مرز بالایی ناحیه اشباع از آب زیرزمینی.
  </div>

  <h3>پرسش و پاسخ</h3>
  <div class="answer">
    <b>۱. آب زیرزمینی چگونه تشکیل می‌شود؟</b><br>
    بخشی از آب باران و برف در زمین نفوذ می‌کند و در فضاهای خالی و شکاف‌ها جمع می‌شود.
  </div>
  <div class="answer">
    <b>۲. آبخوان چیست؟</b><br>
    لایه‌ای از زمین که آب را در خود ذخیره و منتقل می‌کند.
  </div>
  <div class="answer">
    <b>۳. برداشت زیاد از آب‌های زیرزمینی چه نتیجه‌ای دارد؟</b><br>
    پایین رفتن سطح آب زیرزمینی و کاهش ذخیره آب.
  </div>

  <h3>فعالیت و تحقیق</h3>
  <div class="answer">
    <b>نمونه پاسخ: چرا باید در مصرف آب زیرزمینی صرفه‌جویی کنیم؟</b><br>
    چون تجدید این منابع ممکن است زمان زیادی ببرد و برداشت زیاد باعث کاهش ذخیره آن‌ها می‌شود.
  </div>
  <div class="answer">
    <b>نمونه پاسخ: چه عواملی بر نفوذ آب در زمین اثر دارند؟</b><br>
    جنس خاک، اندازه ذرات، میزان فشردگی خاک و وجود شکاف در سنگ‌ها.
  </div>
  <p><b>پایان درس هفتم</b> | تهیه و تنظیم: امیرحسین مواظب</p>
</section>

<section id="quiz">
  <h2 class="section-title">آزمون کوتاه علوم هفتم</h2>

  <div class="quiz-box">
    <p>به سؤال‌ها پاسخ بده و در پایان نتیجه‌ات رو ببین.</p>
    <form id="quizForm">

      <div class="quiz-question">
        <b>۱. کدام مورد به صرفه‌جویی در منابع معدنی کمک می‌کند؟</b>
        <label><input type="radio" name="q1" value="0"> استخراج بیشتر</label>
        <label><input type="radio" name="q1" value="1"> بازیافت فلزها</label>
        <label><input type="radio" name="q1" value="0"> دور ریختن وسایل</label>
      </div>

      <div class="quiz-question">
        <b>۲. عامل اصلی تبخیر آب در طبیعت چیست؟</b>
        <label><input type="radio" name="q2" value="1"> خورشید</label>
        <label><input type="radio" name="q2" value="0"> ماه</label>
        <label><input type="radio" name="q2" value="0"> باد سرد</label>
      </div>

      <div class="quiz-question">
        <b>۳. تبدیل بخار آب به قطره‌های آب چه نام دارد؟</b>
        <label><input type="radio" name="q3" value="0"> تبخیر</label>
        <label><input type="radio" name="q3" value="1"> میعان</label>
        <label><input type="radio" name="q3" value="0"> ذوب</label>
      </div>

      <div class="quiz-question">
        <b>۴. آبخوان چیست؟</b>
        <label><input type="radio" name="q4" value="1"> لایه ذخیره‌کننده و انتقال‌دهنده آب</label>
        <label><input type="radio" name="q4" value="0"> ابر باران‌زا</label>
        <label><input type="radio" name="q4" value="0"> رودخانه سطحی</label>
      </div>

      <div class="quiz-question">
        <b>۵. برداشت بیش از اندازه آب زیرزمینی چه اثری دارد؟</b>
        <label><input type="radio" name="q5" value="0"> افزایش همیشگی آب</label>
        <label><input type="radio" name="q5" value="1"> کاهش ذخیره آب زیرزمینی</label>
        <label><input type="radio" name="q5" value="0"> تشکیل فوری ابر</label>
      </div>

      <button type="button" onclick="checkQuiz()">تصحیح آزمون</button>
    </form>

    <div id="result"></div>
  </div>
</section>

</main>

<footer>
  <strong>AMIR SG</strong><br>
  پروژه آموزشی علوم تجربی پایه هفتم<br>
  طراحی و تهیه: امیرحسین مواظب<br>
  © تمام حقوق این پروژه محفوظ است.
</footer>

<script>
function checkQuiz() {
  const total = 5;
  let score = 0;

  for (let i = 1; i <= total; i++) {
    const answer = document.querySelector(
      'input[name="q' + i + '"]:checked'
    );

    if (answer && answer.value === "1") {
      score++;
    }
  }

  const result = document.getElementById("result");
  result.textContent =
    "نتیجه آزمون: " + score + " از " + total +
    " | درصد: " + Math.round(score / total * 100) + "%";
}
</script>

</body>
</html>
