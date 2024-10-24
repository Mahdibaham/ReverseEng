
خانم‌ها و آقایان، دختران و پسران، بچه‌ها در هر سنی! ما در آستانه سفری هستیم که زندگی شما را برای همیشه تغییر خواهد داد!

مطالب زیادی برای یادگیری وجود دارد تا به درک خوبی از زبان اسمبلی برسیم و بدانیم چرا فهم اصول آن مهم است.

اولین سوال این است که زبان اسمبلی x86 چیست؟ جواب این است که x86 خانواده‌ای از زبان‌های اسمبلی است که با پردازنده‌های سری Intel 8000 سازگار است. زبان‌های اسمبلی x86 برای تولید کد ماشین برای این پردازنده‌ها استفاده می‌شوند و از دستوراتی با نمادهای خاص (mnemonics) تشکیل شده که پردازنده می‌تواند آنها را اجرا کند.

زبان اسمبلی x86 با سیستم‌عامل‌های مختلف کار می‌کند. ما در این آموزش روی زبان اسمبلی لینوکس با استفاده از سینتکس اینتل تمرکز می‌کنیم و همچنین نحوه برنامه‌نویسی به زبان C را یاد می‌گیریم تا بعداً کدها را باز کرده و اسمبلی مربوطه را تحلیل کنیم.

زبان اسمبلی x86 دو نوع سینتکس دارد. سینتکس AT&T که در سیستم‌های یونیکس رایج است و سینتکس اینتل که بیشتر در MS-DOS و ویندوز استفاده می‌شد. در هنگام دیباگ کردن یا باز کردن کد، مخصوصاً در لینوکس یا ویندوز، معمولاً سینتکس اینتل را می‌بینیم. این مهم است، چه در فرمت PE برای فایل‌های ویندوز یا ELF برای فایل‌های لینوکس. تفاوت اصلی این دو در این است که در سینتکس AT&T، منبع قبل از مقصد می‌آید، ولی در اینتل مقصد قبل از منبع است. بعداً بیشتر به این موضوع خواهیم پرداخت.

قبل از اینکه منصرف شوید و بخواهید راه فرار را انتخاب کنید، به یاد داشته باشید که ما این مفاهیم را به تدریج یاد خواهیم گرفت و گیج شدن در این مرحله کاملاً طبیعی است.

ما روی اسمبلی لینوکس تمرکز می‌کنیم زیرا لینوکس روی سخت‌افزارهای متنوعی اجرا می‌شود، از تلفن همراه گرفته تا سرورهای پیچیده تجاری. لینوکس متن‌باز است و نسخه‌های مختلفی دارد. ما از توزیع اوبونتو استفاده خواهیم کرد که رایگان است. در مقابل، ویندوز توسط مایکروسافت کنترل می‌شود و تمامی به‌روزرسانی‌ها و پچ‌های امنیتی از طرف آنها ارائه می‌شود، در حالی که در لینوکس میلیون‌ها متخصص این کار را به‌صورت رایگان انجام می‌دهند!

همچنین، ما بر روی معماری 32 بیتی تمرکز می‌کنیم، زیرا بیشتر بدافزارها برای این معماری نوشته می‌شوند تا سیستم‌های بیشتری را آلوده کنند. برنامه‌ها و بدافزارهای 32 بیتی بر روی سیستم‌های 64 بیتی نیز اجرا می‌شوند، بنابراین باید اصول معماری 32 بیتی را درک کنیم.

در درس بعدی، درباره سیستم اعداد باینری صحبت خواهیم کرد. فنجان قهوه‌تان را آماده کنید، چون به آن نیاز دارید!