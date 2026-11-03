<div align="center">

# HMray Panel
**Advanced 3x-ui Management Platform — independent build**

[English](#english) | [فارسی](#فارسی)

**Repository:** [github.com/amir12120/hmray-panel](https://github.com/amir12120/hmray-panel) · **Upstream:** [HMPanel](https://github.com/neoauroraproject/hmpanel)

</div>

---

<h2 id="english">🇬🇧 English</h2>

HMray Panel is a **professional management layer built specifically on top of native 3x-ui** (an independent build of HMPanel). Designed for VPN Providers, Resellers, and Administrators managing large client bases across multi-panel deployments.

### 📚 Documentation

Setup, operations and API guides live in the [`docs/`](docs) folder of this repository
(some pages still describe features of the upstream editions).

### 🚀 Installation

Execute the following on a fresh Ubuntu (24.04+) or Debian server:
```bash
bash <(curl -fsSL https://raw.githubusercontent.com/amir12120/hmray-panel/main/install.sh)
```
*(Requires: Direct public IP for Let's Encrypt SSL, 1GB RAM, 5GB Disk)*


<summary><b>📸 Screenshots</b></summary>

### Super Admin Dashboard
![Dashboard](docs/images/dashboard-1.png)

### Infrastructure Monitoring
![Monitoring](docs/images/dashboard-2.png)

### Client Management
![Clients](docs/images/clients.png)


### ⚡ Key Features
- **Multi-Panel & Reseller Management:** Control multiple 3x-ui nodes, manage resellers with multi-tier permissions, and set traffic/client limits.
- **Advanced Traffic Accounting:** Real-time collection, automated grace periods, usage-based & allocation-based modes, and secure refund auditing.
- **Native 3x-ui Integration:** Cleanly maps clients to native 3x-ui groups. Attach one client to multiple inbounds seamlessly.
- **Automated Backup System:** Download, upload, and restore PostgreSQL database backups directly from the Web UI.
- **Bulk Operations & Migration Engine:** Efficiently manage clients in bulk and migrate easily from legacy panels (e.g., WhalePanel).

### 💾 Backup & Restore
- **Web UI (New!):** Go to *Settings > System Maintenance* to download, upload, or restore backups with one click.
- **CLI Manager:** Run `sudo hm` to create or restore backups safely via the terminal.

### 🔑 Reset Main Admin Password
Forgot the owner / SUPER_ADMIN password? Reset it from the server (interactive prompt):
```bash
bash <(curl -fsSL https://raw.githubusercontent.com/amir12120/hmray-panel/main/scripts/reset-admin-password.sh)
```
Or via CLI after install/update: `sudo hm admin reset-password` · `sudo hm passwd` · menu option **13**.

Forgot the owner **username** too? `sudo hm admin reset-login` (or `sudo hm reset-login`, menu option **14**) shows the current owner username, then lets you change the username, the password, or both (press Enter to keep either one). The password is typed hidden and asked twice (min 8 characters); a username another admin already uses is rejected, and all existing sessions of the owner are signed out. Run `sudo hm help` for the full command list.

---

<h2 id="فارسی">🇮🇷 فارسی</h2>

اچ‌ام‌ری پنل (HMray Panel) یک **لایه مدیریت حرفه‌ای و پیشرفته برای پنل‌های 3x-ui** است (ساخت مستقل بر پایهٔ HMPanel) که منحصراً برای ارائه‌دهندگان VPN و ادمین‌هایی که چندین سرور و تعداد زیادی کاربر دارند طراحی شده است.

### 📚 مستندات

راهنماهای نصب، بهره‌برداری و API در پوشهٔ [`docs/`](docs) همین مخزن است
(بخشی از صفحه‌ها هنوز قابلیت‌های نسخه‌های اصلی را توضیح می‌دهند).

مخزن: [github.com/amir12120/hmray-panel](https://github.com/amir12120/hmray-panel) · پروژهٔ اصلی: [HMPanel](https://github.com/neoauroraproject/hmpanel)

### 🚀 نصب و راه‌اندازی

دستور زیر را در یک سرور اوبونتو (20.04+) یا دبیان جدید و خام وارد کنید:
```bash
bash <(curl -fsSL https://raw.githubusercontent.com/amir12120/hmray-panel/main/install.sh)
```
*(پیش‌نیازها: آی‌پی پابلیک مستقیم برای دریافت SSL، حداقل 1 گیگابایت رم، 5 گیگابایت فضای ذخیره‌سازی)*

<details>
<summary><b>📸 تصاویر پنل (برای مشاهده کلیک کنید)</b></summary>

### داشبورد سوپر ادمین
![Dashboard](docs/images/dashboard-1.png)

### مانیتورینگ زیرساخت
![Monitoring](docs/images/dashboard-2.png)

### مدیریت کاربران
![Clients](docs/images/clients.png)

</details>

### ⚡ ویژگی‌های کلیدی
- **مدیریت چند پنل و ریسلرها:** کنترل چندین پنل 3x-ui به‌صورت همزمان، تعریف ریسلر با سطوح دسترسی مختلف، همراه با محدودیت ترافیک و تعداد کاربر.
- **حسابداری پیشرفته ترافیک:** محاسبه لحظه‌ای، اعمال قطعی خودکار، حالت‌های مصرفی/تخصیصی، و سیستم امن لاگ و استرداد (Refund Audit) برای جلوگیری از باگ‌های مالی.
- **یکپارچگی با گروه‌های 3x-ui:** تخصیص کاربران به گروه‌های نیتیو و اتصال یک کلاینت به چندین کانفیگ (Inbound) بدون قطعی.
- **سیستم بکاپ‌گیری خودکار:** امکان دانلود، آپلود، و ری‌استور دیتابیس مستقیماً از طریق رابط کاربری (Web UI).
- **عملیات گروهی و مهاجرت آسان:** ابزار حرفه‌ای برای ویرایش و حذف گروهی، به همراه موتور مهاجرت (Migration) قدرتمند از پنل‌های قدیمی (مانند WhalePanel).

### 💾 بکاپ و بازگردانی
- **از طریق پنل کاربری (جدید):** با مراجعه به بخش *تنظیمات > نگهداری سیستم* به راحتی بکاپ‌ها را دانلود، آپلود یا بازگردانی کنید.
- **از طریق ترمینال (CLI):** دستور `sudo hm` را وارد کنید تا به منوی مدیریت سرور و بخش بکاپ دسترسی داشته باشید.

### 🔑 ریست رمز ادمین اصلی
اگر رمز ادمین اصلی (owner / SUPER_ADMIN) را فراموش کردید، روی سرور این دستور تک‌خطی را بزنید:
```bash
bash <(curl -fsSL https://raw.githubusercontent.com/amir12120/hmray-panel/main/scripts/reset-admin-password.sh)
```
یا بعد از نصب/آپدیت: `sudo hm admin reset-password` · `sudo hm passwd` · گزینه **۱۳** منوی `hm`.

**نام کاربری** ادمین اصلی را هم فراموش کرده‌اید؟ دستور `sudo hm admin reset-login` (یا `sudo hm reset-login` یا گزینه **۱۴** منوی `hm`) نام کاربری فعلی ادمین اصلی را نشان می‌دهد و اجازه می‌دهد نام کاربری، رمز یا هر دو را عوض کنید (با Enter هر کدام بدون تغییر می‌ماند). رمز به‌صورت مخفی و دو بار پرسیده می‌شود (حداقل ۸ کاراکتر)، نام کاربری تکراری پذیرفته نمی‌شود و همه‌ی نشست‌های فعلی ادمین اصلی از حساب خارج می‌شوند. فهرست کامل دستورها: `sudo hm help`.

---

<div align="center">

### 💖 Donation / حمایت مالی

**USDT (BEP20):** `0xacA935a5955a756BedaE4738304274EdeE0223D5`

</div>

---

<div align="center">
  <p><strong>HMray Panel</strong> — independent build maintained by <a href="https://github.com/amir12120">amir12120</a></p>
  <p>Based on <a href="https://github.com/neoauroraproject/hmpanel">HMPanel</a> © the HMPanel Team, redistributed with the author's written permission. See <a href="NOTICE.md">NOTICE.md</a>.</p>
</div>
