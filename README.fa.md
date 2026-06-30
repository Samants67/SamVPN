<div align="center" dir="rtl">

<img src="https://raw.githubusercontent.com/iiviirv/irnova-site/main/brand/nova-logo-gradient.svg" width="70" alt="SamVPN">

<div align="left">
  <a href="README.md">🇬🇧 English</a>
</div>

# 🌟 پروژه SamVPN

**SamVPN - توسعه‌یافته توسط سامان تقوی (samants)**

یک پنل گرافیکی کاربردی برای ارائه اشتراک‌های Worker با پروکسی‌های VLESS، Trojan و Warp به همراه زنجیره پروکسی، ارائه‌دهنده تنظیمات کامل DNS، IP تمیز و روتینگ پیشرفته برای کاربران تمامی پلتفرم‌ها با استفاده از هسته‌های Amnezia، Wireguard، Sing-box، Clash/Mihomo و Xray.

[![License](https://img.shields.io/badge/license-MIT-green?style=for-the-badge)](LICENSE)
[![Version](https://img.shields.io/badge/%D9%86%D8%B3%D8%AE%D9%87-3.6.3-blueviolet?style=for-the-badge)](#)

</div>

---

## 🌐 راه‌های ارتباطی

<div align="center">

[![Telegram](https://img.shields.io/badge/✈️%20تلگرام-@irants67-0ea5e9?style=for-the-badge&logo=telegram)](https://t.me/irants67)

</div>

---

## 📖 SamVPN چیست؟

پروژه SamVPN یک **پروکسی شخصی و همه‌کاره برای دور زدن سانسور** است که کاملاً روی Cloudflare Workers — **پلن رایگان** — اجرا می‌شود. این پروژه یک پروکسی قدرتمند (VLESS، Trojan، Shadowsocks روی WebSocket/gRPC/XHTTP) را با **پنل مدیریت کامل دوم‌زبانه** در یک Worker واحد ترکیب کرده است.

**چیزهایی که SamVPN را متفاوت می‌کند:**
- ⚡ **بدون نیاز به زیرساخت** — بدون VPS، بدون دامنه برای شروع
- 🌍 **IP تمیز به‌تفکیک ISP** — بهینه‌سازی خودکار برای هر اپراتور ایرانی
- 👥 **چندکاربره** — لینک اختصاصی با سهمیه، تاریخ انقضا و کنترل روشن/خاموش
- 🤖 **ربات تلگرام** — مدیریت کامل از طریق تلگرام
- 🔗 **زنجیره پروکسی** — SOCKS5، HTTP، HTTPS، TURN، SSTP
- 🛡️ **دورزدن پیشرفته** — ECH، TLS fragment، 0-RTT، fingerprint
- 🧩 **حالت Backend** — اتصال به VPS شخصی Xray/sing-box برای VLESS + تماس تصویری

---

## ⚡ نصب سریع

پس از فورک کردن یا قرار دادن کدها در مخزن خود، می‌توانید تنظیمات مربوط به پروژه را بر اساس مستندات `wrangler.jsonc` شخصی‌سازی کرده و با استفاده از دستورات Wrangler آن را دیپلوی کنید.

---

## 🛰 حالت Backend (VLESS + تماس تصویری/صوتی)

Cloudflare Workers نمی‌تواند پروکسی TCP بومی اجرا کند یا ترافیک UDP را مستقیماً مدیریت کند. برای فعال‌سازی این قابلیت‌ها، SamVPN از **حالت Backend** پشتیبانی می‌کند — ارسال ترافیک به VPS شخصی Xray یا sing-box.

---

## 📋 پیش‌نیازها

- یک **حساب Cloudflare** (رایگان) با Workers فعال
- یک **فضای KV** (با دیپلوی خودکار ساخته می‌شود، یا دستی با Wrangler)
- (اختیاری) Node.js v18+ و Wrangler CLI برای تست محلی

---

## 🧬 قابلیت‌های پنل مدیریتی SamVPN

| قابلیت / Feature | توضیحات و وضعیت |
|------------------|:--:|
| دریافت لینک اشتراک خودکار / Auto subscription link | ✅ |
| فرمت Base64 / Base64 format | ✅ |
| Clash / Mihomo | ✅ |
| sing-box | ✅ |
| Loon | ✅ |
| Surge | ✅ |
| توزیع بار / Load Balancing | ✅ |
| بررسی سلامت / Health Check | ✅ |
| تست پینگ / Ping test | ✅ |
| بهترین کانفیگ / Best config | ✅ |
| QR Code | ✅ |
| نمایش لیست کانفیگ / Display config list | ✅ |
| پروکسی DoH / DoH proxy | ✅ |
| رمزگذاری DNS / DNS encryption | ✅ |
| Load Balance / Failover / Caching DNS | ✅ |
| DNS محلی / Local DNS | ✅ |
| دور زدن تحریم DNS / Anti Sanction DNS | ✅ |
| IP جعلی / Fake DNS | ✅ |
| مسیریابی / GeoIP / GeoSite / Routing | ✅ |
| اتصال مستقیم به سایت ایرانی / Domestic Bypass | ✅ |
| پشتیبانی IPv6 / IPv6 support | ✅ |
| مسدودسازی تبلیغات و بزرگسال / AdBlock + PornBlock | ✅ |
| پورت‌های کلادفلیر / Cloudflare ports | ✅ |
| لینک مستقیم Trojan / Trojan direct link | ✅ |
| لینک مستقیم Clash / Clash direct link | ✅ |
| حالت سراسری SOCKS5 / Global SOCKS5 mode | ✅ |
| حالت سراسری HTTP / Global HTTP mode | ✅ |
| اسکن IP تمیز / Clean Cloudflare IP scanner | ✅ |
| نوتیفیکیشن تلگرام / Telegram notifications | ✅ |
| مدیریت ربات تلگرام / Telegram bot management | ✅ |
| Quantumult X | ✅ |
| تشخیص خودکار کلاینت / Mixed Auto | ✅ |
| Random Path / Wildcard Host | ✅ |
| پنل مدیریت فارسی (RTL) / Admin dashboard | ✅ |
| حالت ساده و پیشرفته / Simple + Advanced mode | ✅ |
| تم تاریک / Dark mode | ✅ |
| ویرایشگر JSON / JSON Config Editor | ✅ |
| مشاهده لاگ / Log Viewer | ✅ |
| بازنشانی تنظیمات / Reset config | ✅ |
| VLESS + Trojan + Shadowsocks | ✅ |
| gRPC + XHTTP transport | ✅ |
| WebSocket Early Data | ✅ |
| mux=0 برای Shadowsocks | ✅ |
| زنجیره SOCKS5 / SOCKS5 chain | ✅ |
| زنجیره HTTP/HTTPS CONNECT | ✅ |
| زنجیره TURN + SSTP | ✅ |
| حالت سراسری HTTPS / TURN / SSTP | ✅ |
| لیست سفید دامنه / Whitelist domains | ✅ |
| زنجیره در لینک اشتراک / Chain in sub link | ✅ |
| TLS 1.3 / 1.2 | ✅ |
| ChaCha20-Poly1305 / AES-GCM | ✅ |
| ClientHello سفارشی / ALPN | ✅ |
| SNI fragment / TLS fragment | ✅ |
| بازگشت به ChaCha20 / Fallback to ChaCha20 | ✅ |
| AES-128/256-GCM (Shadowsocks) | ✅ |
| تشخیص خودکار / کلید جلسه پویا | ✅ |
| بهینه‌سازی آنلاین / API / لیست IP دلخواه | ✅ |
| تولید IP تصادفی / دسته‌بندی نتایج | ✅ |
| ذخیره و جایگزینی نتایج / Save/Override | ✅ |
| بهینه‌سازی IP به‌تفکیک ISP / Per-ISP clean-IP | ✅ |
| Webhook تلگرام / تنظیمات ربات در پنل | ✅ |
| مشاهده مصرف Cloudflare / API Token | ✅ |
| API مصرف سفارشی / Custom Usage API | ✅ |
| لینک مستقیم VLESS + Shadowsocks | ✅ |
| اشتراک با توکن / Subscription with token | ✅ |
| کپی یک‌کلیک / Full clipboard copy | ✅ |
| فضای KV (Config, CF, TG, IPs, Logs) | ✅ |
| ورود با رمز / Auth Cookie | ✅ |
| اعتبارسنجی UUID / Token Auth (MD5) | ✅ |
| مسدودسازی speed test / Speed test block | ✅ |
| متغیرهای محیطی / Environment variables | ✅ |
| پنل واکنش‌گرا فارسی / Persian RTL responsive | ✅ |
| نقشه Leaflet / Toast / Modal | ✅ |
| ماژول‌های جمع‌شونده / SVG icons | ✅ |
| کپی به کلیپ‌بورد / Copy to clipboard | ✅ |
| TCP همزمان / 0-RTT / Concurrent TCP dial | ✅ |
| تجمیع آپلود / داونلود / Uplink/downlink | ✅ |
| محدودیت صف آپلود / Upload queue limit | ✅ |
| Load Balance IP / Proxy Fallback | ✅ |
| لینک اشتراک بدون توکن با فرمت نام‌گذاری شده | ✅ |
| آینه دائمی گیتهاب برای اشتراک | ✅ |
| پنل یکپارچه (Static Assets) | ✅ |
| رابط کاربری دوم‌زبانه + تور راهنما | ✅ |
| مسدودسازی بدافزار / فیشینگ / Cryptominers | ✅ |
| مسدودسازی QUIC | ✅ |
| حالت Backend (VLESS + UDP / تماس تصویری) | ✅ |
| ECH (رمزنگاری SNI) | ✅ |
| Port-spread / Multi-transport | ✅ |
| اعلام خودکار به‌روزرسانی دامنه در تلگرام | ✅ |
| نمودار ترافیک روزانه + تفکیک آپلود/دانلود | ✅ |
| لینک اختصاصی کاربر + سهمیه کل/روزانه + انقضا + روشن/خاموش + غیرفعال خودکار | ✅ |
| لینک اشتراک کاربر با نام کاربری + کلید مخفی | ✅ |
| کش خواندن-پس-از-نوشتن KV برای انتشار آنی تنظیمات | ✅ |
| پشتیبانی NAT64 / انتقال IPv6 | ✅ |
| تغییر رمز پنل + ۲ مرحله‌ای (TOTP) + کد بازیابی | ✅ |
| محدودیت تلاش ورود + مدیریت نشست | ✅ |
| ثبت حساب WARP + لایسنس WARP+ + WoW | ✅ |
| تغییر endpoint WARP + نقاط ایران | ✅ |
| حالت Amnezia WARP + WARP Noise | ✅ |
| حالت یک‌کلیک ایران + گزارش زنده کانفیگ | ✅ |
| پشتیبان‌گیری و بازیابی کامل تنظیمات | ✅ |
| بازگشت میان‌افزاری (گره‌های غیر Cloudflare) | ✅ |
| استخر دامنه خودترمیم + بررسی سلامت | ✅ |
| عبور از کشورها (چین، روسیه، تحریم‌ها) | ✅ |
| قوانین مسیریابی سفارشی | ✅ |
| API مدیریت متمرکز + آمار ناوگان + اعلان همگانی | ✅ |
| خاموش کن سراسری (Kill switch) | ✅ |
| ضربان قلب نمونه + سامانه اعلان‌ها | ✅ |
| پایگاه داده D1 (انتقال از KV) | ✅ |
| ویزارد نصب /install + دیپلوی یک‌کلیکی | ✅ |

---

## 🙏 تشکر

ساخته شده با ❤️ برای اینترنت آزاد و باز.

- [Cloudflare Workers](https://workers.cloudflare.com/)
- [Xray-core](https://github.com/XTLS/xray-core)

---

## مجوز

MIT — فایل [LICENSE](LICENSE) را ببینید.

---

<div align="center">

ساخته شده برای ایران <img src="https://raw.githubusercontent.com/IRNova/Nova-Proxy/main/flag-iran.svg" height="16" alt="Iran" /> — و هرکس که به اینترنت آزاد نیاز دارد.
**هیچ اطلاعاتی از ترافیک شما ذخیره نمی‌شود. پروکسی متعلق به خود شماست.**

📖 [نسخه انگلیسی / English version](README.md)

</div>