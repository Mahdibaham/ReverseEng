## Part 7: Transistors And Memory

در درس گذشته، ما به طور عمیقی به سیستم عددی هگزادسیمال پرداختیم. این هفته می‌خواهم درس را کوتاه نگه‌دارم تا شما بتوانید درس هفته گذشته را دوباره مطالعه کنید. نمی‌توانم تأکید کنم که درک تبدیل‌های عددی هگزادسیمال و توانایی جمع و تفریق دستی آنها چقدر مهم است.

در دنیای واقعی، ما از ماشین‌حساب‌ها استفاده می‌کنیم، در دنیای واقعی از سیستم‌عامل ویندوز استفاده می‌کنیم و مهندسان معکوس حرفه‌ای از دیباگر های گرافیکی مانند IDA Pro و ... استفاده می‌کنند.

سوال این است که چرا بلافاصله به هسته کاری که مهندسان معکوس واقعی انجام می‌دهند نمی‌پردازم؟ جواب ساده است: برای تبدیل شدن به یک مهندس بزرگ، باید به ماشین احترام و درک عمیق داشته باشید. ما هرگز دنیا را تغییر نخواهیم داد مگر اینکه ابتدا آن را به طور کامل درک کنیم. صبر و پافشاری برنده واقعی است.

من بر برنامه‌نویسی لینوکس و کنسولی تمرکز می‌کنم چون بیشتر سرورهای حرفه‌ای از لینوکس استفاده می‌کنند و به همین دلیل بزرگترین تهدید نرم‌افزارهای مخرب است. درک اسمبلی لینوکس به شما این امکان را می‌دهد که فرمت اجرایی قابل حمل ویندوز اسمبلی را به طور عمیق‌تری درک کنید.

حالا که از منبر پایین آمدم، بیایید به اصول اولیه کامپیوترها برگردیم!

وقتی از خودمان می‌پرسیم کامپیوتر چیست، باید به ابتدایی‌ترین سطح ممکن برویم.

کامپیوترهای الکترونیکی به سادگی از سوئیچ‌های ترانزیستوری ساخته شده‌اند. ترانزیستورها کریستال‌های میکروسکوپی سیلیکونی هستند که از خواص الکتریکی سیلیکون برای عمل کردن به عنوان سوئیچ‌ها استفاده می‌کنند. کامپیوترهای مدرن دارای ترانزیستورهای اثر میدان (field-effect transistors) هستند.

بیایید یک مثال از ۳ پین بزنیم. وقتی ولتاژ الکتریکی به پین ۱ اعمال می‌شود، جریان بین پین‌های ۲ و ۳ جریان پیدا می‌کند. وقتی ولتاژ از پین اول برداشته می‌شود، جریان بین پین‌های ۲ و ۳ متوقف می‌شود.

وقتی کمی عقب‌تر می‌رویم، می‌بینیم که دیودها و خازن‌ها نیز وجود دارند که در کنار سوئیچ‌های ترانزیستوری یک سلول حافظه را تشکیل می‌دهند. یک سلول حافظه حداقل جریان را نگه می‌دارد، به طوری که وقتی ولتاژ کمی به پین ورودی آن و ولتاژ مشابهی به پین انتخاب آن بدهیم، ولتاژی در پین خروجی آن ظاهر و حفظ می‌شود. ولتاژ خروجی در وضعیت تنظیم شده خود باقی می‌ماند تا زمانی که ولتاژ از پین ورودی در کنار پین انتخاب برداشته شود.

چرا این مهم است؟ بسیار ساده است، وجود ولتاژ نشان‌دهنده یک باینری ۱ و عدم وجود ولتاژ نشان‌دهنده یک باینری ۰ است؛ بنابراین سلول حافظه یک بیت یا یک عدد باینری که می‌تواند ۱ یا ۰ باشد (به معنی روشن یا خاموش) را نگه می‌دارد.

در درس بعدی درباره بایت‌ها و کلمات صحبت خواهیم کرد.