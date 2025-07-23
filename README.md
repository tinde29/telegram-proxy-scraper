# Telegram Proxy Scraper

[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Python](https://img.shields.io/badge/python-3.9-blue)](https://www.python.org/downloads/)
[![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/tinde29/telegram-proxy-scraper/issues)
[![Proxy Scraper Workflow](https://github.com/tinde29/telegram-proxy-scraper/actions/workflows/scraper.yml/badge.svg)](https://github.com/tinde29/telegram-proxy-scraper/actions/workflows/scraper.yml)
![GitHub last commit](https://img.shields.io/github/last-commit/tinde29/telegram-proxy-scraper)
![GitHub issues](https://img.shields.io/github/issues/tinde29/telegram-proxy-scraper)

**آخرین به‌روزرسانی پروکسی‌ها**: 23 July 2025, 18:58 UTC (به وقت ایران: 22:28)

این پروژه یه اسکریپت پایتون برای جمع‌آوری خودکار پروکسی‌های MTProto تلگرام از منابع متنی و کانال‌های تلگرامه. پروکسی‌ها تو فایل `proxy.txt` ذخیره می‌شن و هر 6 ساعت به‌صورت خودکار به‌روزرسانی می‌شن.

## درباره پروژه

این اسکریپت با استفاده از `requests` و `BeautifulSoup` پروکسی‌های MTProto رو از منابع متنی (مثل فایل‌های خام گیت‌هاب) و صفحات وب کانال‌های تلگرام (`t.me/s/...`) جمع‌آوری می‌کنه. پروکسی‌های تکراری حذف می‌شن و نتیجه تو فایل `proxy.txt` ذخیره می‌شه. فرآیند به‌صورت خودکار با **GitHub Actions** هر 6 ساعت اجرا می‌شه.

## ویژگی‌ها
- جمع‌آوری پروکسی از منابع متنی و کانال‌های تلگرام
- به‌روزرسانی خودکار هر 6 ساعت
- حذف پروکسی‌های تکراری
- بدون نیاز به سرور یا API تلگرام
- مناسب برای کاربرانی که به دنبال پروکسی‌های MTProto فعال هستن

## پیش‌نیازها
- پایتون 3.9
- کتابخونه‌های مورد نیاز: `requests`, `beautifulsoup4`, `pytz`
- فایل `requirements.txt` شامل تمام وابستگی‌هاست.

## نحوه استفاده
1. فایل `proxy.txt` رو از [اینجا](proxy.txt) دانلود کنید.
2. لینک‌های پروکسی (با فرمت `tg://proxy?...`) رو تو کلاینت تلگرام خودتون وارد کنید.
3. برای کپی کردن پروکسی‌های زیر، روی لینک تو ستون "لینک پروکسی" لمس طولانی کنید و گزینه "Copy" رو انتخاب کنید، سپس تو تلگرام پیست کنید.
4. برای به‌روزرسانی دستی، به تب **Actions** تو مخزن برید و روی **Run workflow** کلیک کنید.

## منابع پروکسی
- **منابع متنی**:
  - [MahsaNetConfigTopic](https://raw.githubusercontent.com/MahsaNetConfigTopic/proxy/main/proxies.txt)
  - [ALIILAPRO/MTProtoProxy](https://raw.githubusercontent.com/ALIILAPRO/MTProtoProxy/main/proxy-list.txt)
- **کانال‌های تلگرام**:
  - iporoto, HiProxy, iproxy, iRoProxy, proxyforopeta, IRN_Proxy, MProxy_ir, ProxyHagh, PyroProxy, ProxyMTProto, MTPro_XYZ, vpns, mtmvpn

## نمونه پروکسی‌ها
جدول زیر 30 پروکسی نمونه از فایل `proxy.txt` رو نشون می‌ده. برای کپی کردن لینک پروکسی، روی متن تو ستون "لینک پروکسی" لمس طولانی کنید و "Copy" رو انتخاب کنید:

| #  | سرور (Server)       | پورت (Port) | وضعیت     | لینک پروکسی                     |
|----|---------------------|-------------|-----------|---------------------------------|
| 1 | wait.fiziotr.info | 443 | فعال | `tg://proxy?server=wait.fiziotr.info&port=443&secret=7hYDAQIAAQAB_AMDhuJMOt1tZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 2 | 62.60.179.157 | 343 | فعال | `tg://proxy?server=62.60.179.157&port=343&secret=FgMBAgABAAfwAwOG4kw63Q` |
| 3 | 50.7.85.218 | 443 | فعال | `tg://proxy?server=50.7.85.218&port=443&secret=eee7ce9f4679bfc87bb93390ed56e2c9686170742d6d6972726f722e6f7267` |
| 4 | 195.200.28.26 | 123 | فعال | `tg://proxy?server=195.200.28.26&port=123&secret=eed77db43ee3721f0fcb40a4ff63b5cd276d656469612e737465616d706f77657265642e636f6d` |
| 5 | 011010101101.noirc0re.online | 443 | فعال | `tg://proxy?server=011010101101.noirc0re.online&port=443&secret=35e1c63ac12a5ca4e2866c6e31a5b886` |
| 6 | 89.251.10.4 | 6443 | فعال | `tg://proxy?server=89.251.10.4&port=6443&secret=ee151151151151151151151151151151156d656469612e737465616d706f77657265642e636f6d` |
| 7 | 43.100.108.50 | 443 | فعال | `tg://proxy?server=43.100.108.50&port=443&secret=eee04e6821ae19ca3755852644532a6f61617a7572652e6d6963726f736f66742e636f6d` |
| 8 | LIVE.irpower-b.ir | 443 | فعال | `tg://proxy?server=LIVE.irpower-b.ir&port=443&secret=eed77db43ee3721f0fcb40a4ff63b5cd276D656469612E737465616D706F77657265642E636F6D` |
| 9 | 87.248.134.77 | 200 | فعال | `tg://proxy?server=87.248.134.77&port=200&secret=eeNEgYdJvXrFGRMCIMJdCQ)__` |
| 10 | 150.241.78.70 | 70 | فعال | `tg://proxy?server=150.241.78.70&port=70&secret=7gAA8A8Pd1VV____9QBuLmktLXcuZ28tLS0=` |
| 11 | diamond.hay.aa42hgujoiah-xy1xutr005-2tk.ir | 8443 | فعال | `tg://proxy?server=diamond.hay.aa42hgujoiah-xy1xutr005-2tk.ir&port=8443&secret=7gAA8A8Pd1VV____9QBuLmktLXcuZ28tLS0=` |
| 12 | FOOL.138.60.01-62.ir | 443 | فعال | `tg://proxy?server=FOOL.138.60.01-62.ir&port=443&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 13 | 172.86.66.208.irancell.ir.dijikala.co.uk | 443 | فعال | `tg://proxy?server=172.86.66.208.irancell.ir.dijikala.co.uk&port=443&secret=7hYDAQIAAfADA4biTDrd3E53d3cuZ29vZ2xlLmNvbQ==` |
| 14 | 87.248.132.42 | 200 | فعال | `tg://proxy?server=87.248.132.42&port=200&secret=eed77db43ee3721f0fcb40a4ff63b5cd276D656469612E737465616D706F77657265642E636F6D` |
| 15 | 79.172.228.61 | 70 | فعال | `tg://proxy?server=79.172.228.61&port=70&secret=eed77db43ee3721f0fcb40a4ff63b5cd276D656469612E737465616D706F77657265642E636F6D` |
| 16 | ae.mohs1736.sbs | 4637 | فعال | `tg://proxy?server=ae.mohs1736.sbs&port=4637&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t)__` |
| 17 | SIGNAL.irpower-b.ir | 443 | فعال | `tg://proxy?server=SIGNAL.irpower-b.ir&port=443&secret=eed77db43ee3721f0fcb40a4ff63b5cd276D656469612E737465616D706F77657265642E636F6D` |
| 18 | 1.Ir.ir.ir.ir.ir.zban-mas.info | 8888 | فعال | `tg://proxy?server=1.Ir.ir.ir.ir.ir.zban-mas.info&port=8888&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 19 | htop.link-a4.ir | 443 | فعال | `tg://proxy?server=htop.link-a4.ir&port=443&secret=eed77db43ee3721f0fcb40a4ff63b5cd276D656469612E737465616D706F77657265642E636F6D` |
| 20 | 157.180.127.145 | 44 | فعال | `tg://proxy?server=157.180.127.145&port=44&secret=eeNEgYdJvXrFGRMCIMJdCQ` |
| 21 | 87.248.134.171 | 443 | فعال | `tg://proxy?server=87.248.134.171&port=443&secret=ee0000f00f0f775555fffffff5006e2e696D656469612E737465616D706F77657265642E636F6D)__` |
| 22 | 193.3.190.50 | 85 | فعال | `tg://proxy?server=193.3.190.50&port=85&secret=7gAA8A8Pd1VV____9QBuLmljaGF0Z3B0LmNvbQ` |
| 23 | 142.132.174.75 | 551 | فعال | `tg://proxy?server=142.132.174.75&port=551&secret=eeNEgYdJvXrFGRMCIMJdCQ` |
| 24 | io-ai.time-meli.info | 443 | فعال | `tg://proxy?server=io-ai.time-meli.info&port=443&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t)__` |
| 25 | ir.rayanartist.sbs. | 888 | فعال | `tg://proxy?server=ir.rayanartist.sbs.&port=888&secret=ee0c30628212cbbd7ac519130205525d1569612e737465616d706f77657265642e636f6d****` |
| 26 | 91.99.237.50 | 8888 | فعال | `tg://proxy?server=91.99.237.50&port=8888&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t)__` |
| 27 | 23.88.51.230 | 443 | فعال | `tg://proxy?server=23.88.51.230&port=443&secret=3QAAAAAAAAAAAAAAAAAAAAA=` |
| 28 | 195.2.93.92 | 85 | فعال | `tg://proxy?server=195.2.93.92&port=85&secret=ee0000f00f0f775555fffffff5006e2e69646F776E6C6F61642E77696E646F77737570646174652E636F6D` |
| 29 | 77.238.233.217 | 443 | فعال | `tg://proxy?server=77.238.233.217&port=443&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 30 | Xplor.farda.95.37-68-174.ir | 443 | فعال | `tg://proxy?server=Xplor.farda.95.37-68-174.ir&port=443&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |


> **توجه**: این جدول فقط برای نمایش نمونه‌ست. برای دسترسی به همه پروکسی‌های به‌روز، فایل [proxy.txt](proxy.txt) رو دانلود کنید.

## مشارکت
از مشارکت شما استقبال می‌کنیم! اگه ایده‌ای برای بهبود اسکریپت دارید یا می‌خواید منابع جدیدی اضافه کنید:
1. یه **Issue** تو مخزن باز کنید.
2. یا یه **Pull Request** با تغییرات پیشنهادی بفرستید.

## لایسنس
این پروژه تحت [لایسنس MIT](LICENSE) منتشر شده.

## لینک‌های مفید
- 📄 [لیست پروکسی‌ها](proxy.txt)
- 🚀 [وضعیت GitHub Actions](https://github.com/tinde29/telegram-proxy-scraper/actions)
- ⭐ [ما رو ستاره بدید!](https://github.com/tinde29/telegram-proxy-scraper)

## Stargazers در گذر زمان
[![Stargazers over time](https://starchart.cc/tinde29/telegram-proxy-scraper.svg?variant=adaptive)](https://starchart.cc/tinde29/telegram-proxy-scraper)

---

سپاس از استفاده از **Telegram Proxy Scraper**! اگه سؤالی دارید، تو بخش Issues مطرح کنید. 🌟
