# AAA ExpressVPN Test Lab

### Find working location and protocol combinations on your Windows connection

**AAA Software Studio** · Windows 10/11 x64 · Version **4.2.2**

[فارسی](#فارسی) · [English](#english) · [Release downloads](https://github.com/aaa-software-studio/aaa-expressvpn-test-lab-showcase/releases) · [Report an issue](https://github.com/aaa-software-studio/aaa-expressvpn-test-lab-showcase/issues)

AAA ExpressVPN Test Lab brings location selection, protocol checks, live results and connection reports into one Windows dashboard. It works with the official ExpressVPN application already installed and signed in on your computer.

**Independent project. Not affiliated with or endorsed by ExpressVPN. No VPN account or subscription is included.**

<div dir="rtl" align="right">

## فارسی

### اتصال‌های مناسب شبکهٔ خود را پیدا کنید

وقتی یک لوکیشن یا پروتکل روی شبکهٔ شما وصل نمی‌شود، بررسی تک‌تک گزینه‌ها زمان می‌برد. **AAA ExpressVPN Test Lab** این بررسی را در یک پنل ویندوزی جمع می‌کند: کشورها یا لوکیشن‌های موردنظر را انتخاب کنید، پروتکل‌ها را مشخص کنید و نتیجهٔ تلاش‌های اتصال را در همان صفحه ببینید.

### امکانات

- انتخاب کشورها، لوکیشن‌های تکی یا تمام گزینه‌هایی که برنامهٔ رسمی ارائه می‌کند.
- بررسی پروتکل‌های Automatic، Lightway UDP/TCP، WireGuard و OpenVPN TCP/UDP، با توجه به پشتیبانی نسخهٔ نصب‌شدهٔ ExpressVPN.
- تنظیم تعداد تلاش‌ها، مهلت اتصال، تأخیر تلاش مجدد و مدت بررسی پایداری.
- نمایش اتصال‌های تأییدشده، تمام تلاش‌ها و گزارش تشخیصی زنده.
- کپی نتایج و خروجی CSV و JSON برای بررسی شخصی.
- بررسی اختیاری HTTPS و هشدار پیش از شروع تغییر اتصال.

«تأییدشده» یعنی وضعیت برنامهٔ رسمی متصل باشد، لوکیشن گزارش‌شده تطابق داشته باشد، IP عمومی نسبت به حالت قطع تغییر کند و در صورت فعال‌بودن، بررسی HTTPS هم موفق شود. زمان نمایش‌داده‌شده، معیار سرعت دانلود یا رتبه‌بندی تمام سرورهای فیزیکی نیست.

### دانلود و اجرا

۱. بستهٔ **Windows Portable** را از بخش [Releases](https://github.com/aaa-software-studio/aaa-expressvpn-test-lab-showcase/releases) بگیرید و کامل استخراج کنید. اگر یک ZIP دیگر داخل دانلود بود، آن را هم استخراج کنید.

۲. برنامهٔ رسمی ExpressVPN را نصب و باز کنید و در پنجرهٔ خود ExpressVPN وارد حساب فعال خود شوید.

۳. فایل <code dir="ltr">AAA-ExpressVPN-TestLab.exe</code> را اجرا کنید. نصب Python لازم نیست؛ پوشهٔ همراه EXE باید کنارش بماند.

۴. تنظیمات را انتخاب کنید و قبل از Start Scan هشدار تغییر اتصال را بخوانید. در صورت درخواست ویندوز، دسترسی مدیر برای کنترل برنامهٔ رسمی لازم می‌شود.

### پیش از اسکن بدانید

شروع آزمایش می‌تواند اتصال VPN فعلی را قطع کند. برنامه پس از پایان، توقف حین اسکن یا خطای مدیریت‌شده، برای قطع اتصال اقدام و وضعیت را بررسی می‌کند؛ اتصال و پروتکل قبلی را خودکار بازنمی‌گرداند. بستن اجباری برنامه، خاموشی یا خرابی سیستم می‌تواند مانع پاک‌سازی شود.

خطاهای پیش‌بررسی و انصراف پیش از آغاز تغییر اتصال، در آزمون‌های شبیه‌سازی‌شده بدون قطع VPN بررسی شده‌اند. هنگام آزمایش، کار وابسته به اتصال پیوسته انجام ندهید.

### وضعیت بررسی

ساخت EXE روی ویندوز و اجرای **۴۵ آزمون خودکار** موفق بوده است. سازنده بازشدن رابط همین نسخهٔ ۴.۲.۲ روی کامپیوتر خود را با تصویر تأیید کرده است. این نتیجه به معنی آزمون کامل اسکن واقعی همین فایل، سازگاری همهٔ سیستم‌ها یا بررسی امنیت مستقل نیست. فایل امضای دیجیتال ناشر ندارد.

### حریم خصوصی

تنظیمات و خروجی‌ها روی دستگاه و در مسیر <code dir="ltr">%LOCALAPPDATA%\AAA-ExpressVPN-TestLab</code> ذخیره می‌شوند. گزارش‌ها ممکن است IP عمومی، نام لوکیشن، زمان و متن خطای برنامهٔ رسمی را داشته باشند؛ پیش از اشتراک‌گذاری آن‌ها را پاک‌سازی کنید.

بررسی IP به ipify و در صورت نیاز Amazon checkip درخواست می‌فرستد؛ بررسی اختیاری HTTPS از Cloudflare استفاده می‌کند. این سرویس‌ها IP مبدأ درخواست را می‌بینند. رفتار شبکهٔ خود ExpressVPN مستقل از این ابزار است.

### بازخورد و سازنده

برای گزارش مشکل فعلاً از [GitHub Issues](https://github.com/aaa-software-studio/aaa-expressvpn-test-lab-showcase/issues) استفاده کنید؛ رمز، اطلاعات حساب و گزارش پاک‌سازی‌نشده نفرستید. راه ارتباطی مستقیم استودیو بعداً اضافه می‌شود.

ساخته‌شده از ایدهٔ سازنده با کمک هوش مصنوعی در **AAA Software Studio**. این مخزن برای معرفی، مستندات و دانلود نسخهٔ اجرایی است؛ سورس توسعه خصوصی می‌ماند.

</div>

## English

### A practical dashboard for ExpressVPN connection checks

Select countries or individual locations, choose protocols, and inspect connection attempts in one desktop interface. The utility controls the locally installed official `expressvpnctl.exe`; it does not provide VPN infrastructure or credentials.

- Search and select locations returned by the installed official client.
- Configure attempts, connection timeouts, retries and post-connection observation.
- Inspect verified connections, all attempts and diagnostic output.
- Copy results or export CSV/JSON reports locally.
- Enable an optional HTTPS check and review a warning before connection changes.

Verification combines official connected status, matching location and a public IP change against a disconnected baseline, plus HTTPS when enabled. It does not benchmark bandwidth, enumerate every physical server or establish that a failed location is blocked.

### Requirements and installation

Windows 10/11 x64, a compatible official ExpressVPN Windows client with `expressvpnctl.exe`, and your own active account. Extract the complete Windows Portable package and run **AAA-ExpressVPN-TestLab.exe**. **Python installation is not required. Keep the bundled support folder beside the EXE.**

Use the manually attached **Windows Portable** release asset. GitHub's automatic **Source code** archives contain only this documentation repository, not the application.

### Connection behavior and testing

Scanning intentionally changes VPN connections and does not restore the original connection or protocol. After connection changes begin, finish, Stop and handled errors attempt a disconnect and verify status. Forced termination, system shutdown or crashes can prevent cleanup. Read the confirmation before starting.

The Windows build and 45 automated tests passed. The creator supplied a screenshot confirming that the 4.2.2 GUI opened on their Windows PC. Full live VPN regression testing of this binary, broad Windows compatibility and independent security review are not claimed. The binary is unsigned.

### Data, attribution and feedback

Settings and reports are stored under `%LOCALAPPDATA%\AAA-ExpressVPN-TestLab`. Reports may contain public IPs, timestamps and CLI diagnostics. Public-IP requests use ipify with Amazon checkip as fallback; optional HTTPS checks use Cloudflare. These endpoints observe request source IPs.

The distributed package includes third-party notices and country-data provenance. Retain those notices. No open-source license for the private application is granted by this showcase. ExpressVPN names and marks belong to their respective owners.

For now, use [GitHub Issues](https://github.com/aaa-software-studio/aaa-expressvpn-test-lab-showcase/issues) for feedback, with private details removed. A direct studio contact will be added later.

Built by [AAA Software Studio](https://github.com/aaa-software-studio) from the creator's idea with AI assistance.
