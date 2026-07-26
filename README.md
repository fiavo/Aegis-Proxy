<div align="center">

# 🛡️ Aegis Proxy

**پروکسی هوشمند و ضدسانسور روی Cloudflare Workers**

[![License](https://img.shields.io/badge/license-MIT-green?style=for-the-badge)](LICENSE)
[![Version](https://img.shields.io/badge/version-1.0.0-blueviolet?style=for-the-badge)](https://github.com/fiavo/Aegis-Proxy)
[![Stars](https://img.shields.io/github/stars/fiavo/Aegis-Proxy?style=for-the-badge&color=0ea5e9)](https://github.com/fiavo/Aegis-Proxy)

</div>

---

## 🌟 ویژگی‌ها

- ⚡ **سرعت بالا** - اجرای کامل روی Cloudflare Workers
- 🔒 **امنیت پیشرفته** - رمزنگاری قوی و بدون لاگ
- 🌍 **IP تمیز** - بهینه‌سازی خودکار برای ISPهای ایرانی
- 👥 **چندکاربره** - مدیریت کاربران با سهمیه و تاریخ انقضا
- 🤖 **ربات تلگرام** - مدیریت کامل از طریق تلگرام
- 📱 **چندپلتفرمه** - پشتیبانی از تمام دستگاه‌ها
- 🆓 **رایگان** - اجرا روی پلن رایگان Cloudflare

---

## 📋 پروتکل‌های پشتیبانی شده

| پروتکل | توضیح |
|--------|--------|
| VLESS | سریع و امن |
| Trojan | قابل اعتماد |
| Shadowsocks | کلاسیک و پایدار |
| WireGuard | مدرن و سریع |
| Xray | انعطاف‌پذیر |

---

## 🚀 شروع سریع

### پیش‌نیازها

- [Node.js](https://nodejs.org/) نسخه 18+
- [اکانت Cloudflare](https://www.cloudflare.com/) (رایگان)
- [Wrangler CLI](https://developers.cloudflare.com/workers/wrangler/)

### نصب و استقرار

```bash
# ۱. کلون کردن پروژه
git clone https://github.com/fiavo/Aegis-Proxy.git
cd Aegis-Proxy

# ۲. نصب وابستگی‌ها
npm install

# ۳. ورود به Cloudflare
wrangler login

# ۴. ایجاد دیتابیس
wrangler d1 create aegis-proxy-db

# ۵. ویرایش wrangler.jsonc
# database_id رو از مرحله ۴ کپی کنید

# ۶. استقرار
wrangler deploy

# ۷. تنظیم اولیه
# لینک Worker رو باز کنید و به /install برید
```

---

## 📖 راهنما

### 🌐 دسترسی به پنل

پس از استقرار، پنل مدیریت در دسترس خواهد بود:

```
https://your-worker.workers.dev/install
```

### 👤 ایجاد کاربر

1. وارد پنل شوید
2. به بخش "کاربران" بروید
3. کاربر جدید اضافه کنید
4. لینک اختصاصی رو کپی کنید

### 📱 اتصال در تلگرام

1. لینک ساب‌سکریپشن رو کپی کنید
2. در تلگرام ارسال کنید
3. اتصال خودکار برقرار میشه

---

## ⚙️ تنظیمات پیشرفته

### ربات تلگرام

```bash
# در بخش Settings پنل
TELEGRAM_BOT_TOKEN: توکن ربات
TELEGRAM_ADMINS: آیدی ادمین
```

### WARP

```bash
# فعال‌سازی WARP
Settings → WARP → Enable
```

### دامنه اختصاصی

```bash
# اضافه کردن دامنه
wrangler route add aegis-proxy.ir/*
```

---

## 🔧 عیب‌یابی

### مشکل اتصال

```bash
# لاگ‌ها رو چک کنید
wrangler tail
```

### مشکل دیتابیس

```bash
# دیتابیس رو لیست کنید
wrangler d1 list
```

### آپدیت خودکار

```bash
# آپدیت دستی
wrangler deploy
```

---

## 📊 عملکرد

| ویژگی | مقدار |
|-------|-------|
| ⏱️ پینگ | < 50ms |
| 🚀 سرعت | > 100Mbps |
| 💾 حافظه | < 128MB |
| 👥 کاربران همزمان | > 1000 |

---

## 🤝 مشارکت

ما از مشارکت شما استقبال می‌کنیم!

1. Fork کنید
2. Branch جدید بسازید
3. تغییرات رو commit کنید
4. Pull Request بزنید

---

## 📄 لایسنس

این پروژه تحت لایسنس [MIT](LICENSE) منتشر شده است.

---

## 🙏 قدردانی

- [Cloudflare](https://www.cloudflare.com/) - زیرساخت رایگان
- [fiavo](https://github.com/fiavo) - پروژه اصلی
- جامعه توسعه‌دهندگان ایرانی

---

<div align="center">

**🛡️ Aegis Proxy - محافظت از حریم خصوصی شما**

</div>
