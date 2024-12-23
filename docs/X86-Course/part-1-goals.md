## Part 1: Goals

برای بحث در مورد مهندسی معکوس بدافزار، باید مفهوم تحلیل بدافزار را درک کنیم. تحلیل بدافزار به بررسی و درک اطلاعاتی اشاره دارد که برای پاسخ به نفوذهای شبکه‌ای ضروری است.

این آموزش کوتاه با مفاهیم پایه مهندسی معکوس بدافزار شروع می‌شود و به بررسی مقدماتی زبان اسمبلی می‌رسد.

کلید اصلی این بحث در تجزیه و تحلیل فایل‌های مشکوک بدافزار و نحوه شناسایی آن‌ها در شبکه شما و نهایتاً مهار کردن آن‌ها است.

پس از شناسایی کامل فایل‌های مورد نیاز برای تحلیل عمیق‌تر، مهم است که امضاهایی برای شناسایی عفونت‌های بدافزاری در تمام شبکه خود توسعه دهید. این شبکه می‌تواند یک شبکه محلی خانگی یا یک شبکه بزرگ شرکتی باشد که در آن تحلیل بدافزار ضروری است تا امضاهای مبتنی بر میزبان و شبکه ایجاد شود.

برای شروع با مفهوم امضای مبتنی بر میزبان، باید بدانیم که این امضاها برای شناسایی کدهای مخرب در یک دستگاه هدف استفاده می‌شوند. امضاهای مبتنی بر میزبان به عنوان نشانه‌هایی شناخته می‌شوند که می‌توانند فایل‌هایی را که توسط کد آلوده ایجاد یا ویرایش شده‌اند، شناسایی کنند. این کدها می‌توانند تغییرات مخفی در رجیستری کامپیوتر ایجاد کنند. این مسئله کاملاً با امضاهای آنتی‌ویروس متفاوت است، زیرا آنتی‌ویروس‌ها بیشتر بر روی آنچه که بدافزار انجام می‌دهد تمرکز دارند تا ساختار خود بدافزار. این ویژگی باعث می‌شود که آن‌ها در یافتن بدافزارهایی که می‌توانند منتقل شوند یا از رسانه حذف شده‌اند، مؤثرتر باشند.

در مقابل، امضاهای شبکه برای شناسایی کدهای مخرب با بررسی ترافیک شبکه استفاده می‌شوند. مهم است که ابزارهایی مانند `Wireshark` و مشابه آن در این تحلیل مؤثر هستند.

پس از شناسایی این امضاهای ذکر شده، مرحله بعدی شناسایی این است که بدافزار واقعاً چه کار می‌کند.

____

در درس بعدی ما به بررسی تکنیک‌های تحلیل بدافزار خواهیم پرداخت.