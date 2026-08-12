# 💜Netra Panel
<p align="center">
  <img src="https://img.shields.io/badge/Cloudflare-Workers-F38020?style=for-the-badge&logo=cloudflare&logoColor=white" alt="Cloudflare Workers">
  <img src="https://img.shields.io/badge/Protocol-VLESS-00ADD8?style=for-the-badge&logo=v&logoColor=white" alt="VLESS">
  <img src="https://img.shields.io/badge/Protocol-Trojan-00ADD8?style=for-the-badge&logo=trojan&logoColor=white" alt="Trojan">
</p>
یک پنل پروکسی رایگان، خودمیزبان و قدرتمند بر بستر Cloudflare Workers

**زبان / Language / Язык / 语言:** [فارسی](#فارسی) | [English](#english) | [Русский](#русский) | [中文](#中文)

---

## فارسی

### پنل Netra

یک پنل پروکسی VLESS / Trojan رایگان و خودمیزبان که کاملاً روی **Cloudflare Workers** اجرا می‌شه. بدون نیاز به VPS، بدون نگهداری سرور، بدون هزینه‌ی ماهانه — در چند دقیقه دیپلوی کنید و همه‌چیز رو از یک پنل تمیز مدیریت کنید.

[گزارش باگ](https://github.com/netrair/issues) · [درخواست ویژگی جدید](https://github.com/netrair/issues) · [پشتیبانی تلگرام](https://t.me/NetraIR)

---

### ✨ ویژگی‌ها

* ⚡ **کاملاً روی Cloudflare Workers اجرا می‌شه** — بدون VPS، بدون Docker، بدون سروری که نیاز به آپدیت یا ری‌استارت داشته باشه
* پشتیبانی از پروتکل‌های **VLESS** و **Trojan**
* پشتیبانی از **Warp / Warp Pro** برای مسیرهای اضافی
* لینک سابسکریپشن برای کلاینت‌های Xray-core، sing-box، Clash و WireGuard (مثل v2rayNG، Streisand، Clash Meta، Hiddify، NekoBox و...)
* ️ تنظیمات Fragment و نویز برای عبور بهتر از فیلترینگ‌های سخت‌گیرانه
* ️ **پنل وب کامل** — همه‌چیز (UUID، پسورد، پورت‌ها، DNS، قوانین مسیریابی، لیست‌های bypass/block) بدون نیاز به دست‌زدن به کد قابل مدیریته
* **دیپلوی با یک کلیک** — بلافاصله بعد از دیپلوی با مقادیر پیش‌فرض کار می‌کنه، بدون نیاز به Wizard جداگانه
* **رمز پنل اختیاریه** — می‌تونید پنل رو با رمز محافظت کنید یا اگه فقط خودتون آدرسش رو دارید، ردش کنید

---

### نصب و دیپلوی

1. روی دکمه‌ی **Deploy to Cloudflare Workers** بزنید، یا یک Worker جدید توی [داشبورد Cloudflare](https://dash.cloudflare.com) بسازید.
2. محتوای فایل `worker.js` رو کپی و توی ویرایشگر Worker جای‌گذاری و دیپلوی کنید.
3. یک **KV Namespace** با نام `kv` به Worker متصل کنید (از مسیر Settings → Variables → KV Namespace Bindings).
4. آدرس Worker خودتون رو باز کنید و برید به `/panel` — بار اول ازتون خواسته می‌شه یک رمز برای پنل تعیین کنید یا ردش کنید.

همین! پنل بلافاصله با تنظیمات پیش‌فرض کار می‌کنه. بعداً می‌تونید همه‌چیز (UUID، پسورد Trojan، مسیر امن، پورت‌ها، قوانین مسیریابی و...) رو از داخل پنل شخصی‌سازی کنید.

---

### نکات امنیتی

* اگه گزینه‌ی **Skip password** رو بزنید، هر کسی که آدرس Workerتون رو داشته باشه می‌تونه وارد پنل بشه. این کار رو فقط برای دیپلوی شخصی/تستی بدید.
* قبل از اشتراک‌گذاری لینک سابسکریپشن، UUID/پسورد Trojan/مسیر امن پیش‌فرض رو از پنل عوض کنید.
* با آدرس Workerتون مثل یک اطلاعات محرمانه رفتار کنید — این آدرس دروازه‌ی ورود به پنلتونه.

---

### پشتیبانی

سوال یا مشکلی دارید؟ توی تلگرام پیام بدید: **[@NetraIR](https://t.me/NetraIR)**

---

## English

### Netra Panel

A free, self-hosted VLESS / Trojan proxy panel that runs entirely on **Cloudflare Workers**. No VPS. No server maintenance. No monthly cost — deploy in minutes and manage everything from a clean web panel.

[Report a Bug](https://github.com/netrair/issues) · [Request a Feature](https://github.com/netrair/issues) · [Telegram Support](https://t.me/NetraIR)

---

### ✨ Features

* ⚡ **Runs on Cloudflare Workers** — no VPS, no Docker, no server to patch or reboot
* **VLESS & Trojan** protocol support out of the box
* **Warp / Warp Pro** integration for extra routing options
* **Subscription links** for Xray-core, sing-box, Clash, and WireGuard-based clients (v2rayNG, Streisand, Clash Meta, Hiddify, NekoBox, and more)
* ️ **Fragment & noise settings** to help traffic blend in on restrictive networks
* ️ **Full web panel** — manage everything (UUID, password, ports, DNS, routing rules, bypass/block lists) without touching code
* **One-click deploy** — works with sensible defaults right after deployment, no separate setup wizard required
* **Optional panel password** — protect your panel, or skip it if you're the only one with the URL

---

### Deploy

1. Click **Deploy to Cloudflare Workers**, or manually create a new Worker in your [Cloudflare dashboard](https://dash.cloudflare.com).
2. Paste the contents of `worker.js` into the Worker editor and deploy.
3. Add a **KV Namespace** binding named `kv` to the Worker (Settings → Variables → KV Namespace Bindings).
4. Open your Worker's URL and go to `/panel` — you'll be prompted to set a panel password (or skip it) on first visit.

That's it — the panel works immediately with built-in defaults. You can customize everything (UUID, Trojan password, secure path, ports, routing rules, etc.) from inside the panel afterward.

---

### Security notes

* If you choose **Skip password**, anyone with your Worker URL can access the panel. Only do this for a private/testing deployment.
* Change the default UUID/Trojan password/secure path from the panel before sharing your subscription link with anyone.
* Treat your Worker URL like a secret — it's the entry point to your panel.

---

### Support

Questions or issues? Reach out on Telegram: **[@NetraIR](https://t.me/NetraIR)**

---

## Русский

### Netra Panel

Бесплатная self-hosted панель для прокси VLESS / Trojan, которая полностью работает на **Cloudflare Workers**. Без VPS. Без обслуживания сервера. Без ежемесячной платы — разверните за пару минут и управляйте всем через удобную веб-панель.

[Сообщить об ошибке](https://github.com/netrair/issues) · [Предложить функцию](https://github.com/netrair/issues) · [Поддержка в Telegram](https://t.me/NetraIR)

---

### ✨ Возможности

* ⚡ **Работает на Cloudflare Workers** — не нужен VPS, Docker или обслуживание сервера
* Поддержка протоколов **VLESS и Trojan** из коробки
* Интеграция с **Warp / Warp Pro** для дополнительных маршрутов
* **Ссылки подписки** для Xray-core, sing-box, Clash и WireGuard-клиентов (v2rayNG, Streisand, Clash Meta, Hiddify, NekoBox и др.)
* ️ Настройки **Fragment и noise** для лучшего обхода жёсткой фильтрации трафика
* ️ **Полноценная веб-панель** — управляйте всем (UUID, пароль, порты, DNS, правила маршрутизации, списки bypass/block) без изменения кода
* **Развёртывание в один клик** — работает с готовыми настройками сразу после деплоя, отдельный мастер настройки не требуется
* **Пароль панели — по желанию** — защитите панель паролем или пропустите этот шаг, если только у вас есть ссылка

---

### Установка

1. Нажмите **Deploy to Cloudflare Workers** или создайте новый Worker вручную в [панели Cloudflare](https://dash.cloudflare.com).
2. Вставьте содержимое файла `worker.js` в редактор Worker и разверните его.
3. Добавьте привязку **KV Namespace** с именем `kv` к Worker (Settings → Variables → KV Namespace Bindings).
4. Откройте URL вашего Worker и перейдите на `/panel` — при первом входе будет предложено задать пароль панели (или пропустить этот шаг).

Готово — панель сразу работает со встроенными значениями по умолчанию. Позже вы сможете настроить всё (UUID, пароль Trojan, секретный путь, порты, правила маршрутизации и т.д.) прямо в панели.

---

### Заметки по безопасности

* Если выбрать **Skip password**, любой, у кого есть ссылка на ваш Worker, сможет открыть панель. Используйте это только для личного/тестового развёртывания.
* Перед тем как делиться ссылкой подписки, измените в панели стандартный UUID/пароль Trojan/секретный путь.
* Относитесь к URL вашего Worker как к секретной информации — это точка входа в вашу панель.

---

### Поддержка

Вопросы или проблемы? Пишите в Telegram: **[@NetraIR](https://t.me/NetraIR)**

---

## 中文

### Netra Panel

一个完全运行在 **Cloudflare Workers** 上的免费自托管 VLESS / Trojan 代理面板。无需 VPS，无需维护服务器，无需每月付费 —— 几分钟内即可部署完成，通过简洁的网页面板管理一切。

[提交 Bug](https://github.com/netrair/issues) · [功能建议](https://github.com/netrair/issues) · [Telegram 支持](https://t.me/NetraIR)

---

### ✨ 功能特点

* ⚡ **完全运行在 Cloudflare Workers 上** —— 无需 VPS、Docker，也无需维护或重启服务器
* 开箱即用支持 **VLESS 和 Trojan** 协议
* 集成 **Warp / Warp Pro**，提供更多路由选择
* 为 Xray-core、sing-box、Clash 和 WireGuard 客户端提供**订阅链接**（v2rayNG、Streisand、Clash Meta、Hiddify、NekoBox 等）
* ️ **Fragment 与噪声设置**，帮助流量更好地绕过严格的网络封锁
* ️ **完整的网页面板** —— 无需接触代码即可管理一切（UUID、密码、端口、DNS、路由规则、绕过/屏蔽列表）
* **一键部署** —— 部署后立即使用内置默认配置即可运行，无需单独的设置向导
* **面板密码可选** —— 可为面板设置密码保护，若只有你自己掌握链接，也可以跳过

---

### 部署方法

1. 点击 **Deploy to Cloudflare Workers**，或前往你的 [Cloudflare 控制台](https://dash.cloudflare.com) 手动创建一个新的 Worker。
2. 将 `worker.js` 的内容复制并粘贴到 Worker 编辑器中，然后部署。
3. 为该 Worker 添加一个名为 `kv` 的 **KV Namespace** 绑定（路径：Settings → Variables → KV Namespace Bindings）。
4. 打开你的 Worker 地址并访问 `/panel` —— 首次访问时会提示你设置面板密码（也可以选择跳过）。

就这么简单 —— 面板会立即使用内置默认配置正常运行。之后你可以在面板内自行自定义所有设置（UUID、Trojan 密码、安全路径、端口、路由规则等）。

---

### 安全提示

* 如果选择 **Skip password（跳过密码）**，任何拥有你 Worker 地址的人都可以访问面板。请仅在个人/测试部署时使用此选项。
* 在分享订阅链接前，请务必在面板中修改默认的 UUID / Trojan 密码 / 安全路径。
* 请像对待机密信息一样对待你的 Worker 地址 —— 它是进入你面板的入口。

---

### 获取支持

有问题或遇到故障？请通过 Telegram 联系：**[@NetraIR](https://t.me/NetraIR)**

---

Made with ❤️ for a freer internet.
.
