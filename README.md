# Telegram Proxy Scraper

[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Python](https://img.shields.io/badge/python-3.9-blue)](https://www.python.org/downloads/)
[![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/tinde29/telegram-proxy-scraper/issues)
[![Proxy Scraper Workflow](https://github.com/tinde29/telegram-proxy-scraper/actions/workflows/scraper.yml/badge.svg)](https://github.com/tinde29/telegram-proxy-scraper/actions/workflows/scraper.yml)
![GitHub last commit](https://img.shields.io/github/last-commit/tinde29/telegram-proxy-scraper)
![GitHub issues](https://img.shields.io/github/issues/tinde29/telegram-proxy-scraper)

**آخرین به‌روزرسانی پروکسی‌ها**: 23 July 2025, 06:59 UTC (به وقت ایران: 10:29)

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
| 1 | 140.233.187.210 | 443 | فعال | `tg://proxy?server=140.233.187.210&port=443&secret=eed77db43ee3721f0fcb40a4ff63b5cd276d656469612e737465616d706f77657265642e636f6d` |
| 2 | 194.26.141.32 | 443 | فعال | `tg://proxy?server=194.26.141.32&port=443&secret=ee100404ff0f48064fffffff9001b8696d696d656469612e737465616d706f77657265642e636f6d` |
| 3 | 157.180.67.46 | 44 | فعال | `tg://proxy?server=157.180.67.46&port=44&secret=eeNEgYdJvXrFGRMCIMJdCQ` |
| 4 | 91.99.138.108 | 155 | فعال | `tg://proxy?server=91.99.138.108&port=155&secret=7hYDAQIAAQAH8AMDhuJMOt1tZWRpYS5zdGVhbXBvd2VyZWQuY29tbWVkaWEuc3RlYW1wb3dlcmVkLmNvbQ)__` |
| 5 | 418db.www.google.com.alphard.cfd | 2310 | فعال | `tg://proxy?server=418db.www.google.com.alphard.cfd&port=2310&secret=7jK5IN_7UWQwKOL2uHjU6sEgICAgICAgICAgICAgICA)🫥[**` |
| 6 | newmuozick.co.uk | 443 | فعال | `tg://proxy?server=newmuozick.co.uk&port=443&secret=FgMBAgABAAH8AwOG4kw63Q` |
| 7 | 62.60.176.30 | 443 | فعال | `tg://proxy?server=62.60.176.30&port=443&secret=7hAQEP8PSAZT____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 8 | bezan.sitemcinet.co.uk | 443 | فعال | `tg://proxy?server=bezan.sitemcinet.co.uk&port=443&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 9 | 91.99.166.4 | 8888 | فعال | `tg://proxy?server=91.99.166.4&port=8888&secret=7gAA8A8Pd1VV////9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 10 | 62.60.176.253 | 443 | فعال | `tg://proxy?server=62.60.176.253&port=443&secret=eed77db43ee3721f0fcb40a4ff63b5cd276D656469612E737465616D706F77657265642E636F6D` |
| 11 | net-meli.bozorgavar-game.ir. | 9741 | فعال | `tg://proxy?server=net-meli.bozorgavar-game.ir.&port=9741&secret=ee0000f00f0f775555fffffff5006e2e696d656469612e737465616d706f77657265642e636f6d)__` |
| 12 | 87.248.132.21 | 70 | فعال | `tg://proxy?server=87.248.132.21&port=70&secret=eed77db43ee3721f0fcb40a4ff63b5cd276D656469612E737465616D706F77657265642E636F6D` |
| 13 | 62.60.177.75 | 443 | فعال | `tg://proxy?server=62.60.177.75&port=443&secret=7hYDAQIAAQAH8AMDhuJMOt1tZWRpYS5zdGVhbXBvd2VyZWQuY29tbWVkaWEuc3RlYW1wb3dlcmVkLmNvbQ` |
| 14 | 193.3.190.47 | 85 | فعال | `tg://proxy?server=193.3.190.47&port=85&secret=7gAA8A8Pd1VV____9QBuLmljaGF0Z3B0LmNvbQ` |
| 15 | systemfull.gjesus.info | 443 | فعال | `tg://proxy?server=systemfull.gjesus.info&port=443&secret=ee1603010200010001fc030386e24c3add6d656469612e737465616d706f77657265642e636f6d` |
| 16 | Iranam.new-visioncity.ir. | 443 | فعال | `tg://proxy?server=Iranam.new-visioncity.ir.&port=443&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 17 | 140.233.187.60 | 443 | فعال | `tg://proxy?server=140.233.187.60&port=443&secret=eed77db43ee3721f0fcb40a4ff63b5cd276d656469612e737465616d706f77657265642e636f6d` |
| 18 | 31.184.172.121 | 2086 | فعال | `tg://proxy?server=31.184.172.121&port=2086&secret=1f9fdd1eddffba2661772fa299eef89c` |
| 19 | www.wwweror.space. | 888 | فعال | `tg://proxy?server=www.wwweror.space.&port=888&secret=ee0c30628212cbbd7ac519130205525d1569612e737465616d706f77657265642e636f6d` |
| 20 | 213.145.71.150 | 70 | فعال | `tg://proxy?server=213.145.71.150&port=70&secret=7gffffffff_f_Adkb3dubG9hZC53aW5kb3dzdXBkYXRlLmNvbQ` |
| 21 | 87.229.100.159 | 443 | فعال | `tg://proxy?server=87.229.100.159&port=443&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 22 | 87.248.132.88 | 200 | فعال | `tg://proxy?server=87.248.132.88&port=200&secret=eeNEgYdJvXrFGRMCIMJdCQ)__` |
| 23 | 204.76.203.36 | 443 | فعال | `tg://proxy?server=204.76.203.36&port=443&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 24 | 93.88.205.35 | 85 | فعال | `tg://proxy?server=93.88.205.35&port=85&secret=7gAA8A8Pd1VV__9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 25 | 62.60.177.195 | 9741 | فعال | `tg://proxy?server=62.60.177.195&port=9741&secret=ee0000f00f0f775555fffffff5006e2e696d656469612e737465616d706f77657265642e636f6d` |
| 26 | halftime.parsintalk.ir | 443 | فعال | `tg://proxy?server=halftime.parsintalk.ir&port=443&secret=7hYDAQIAAQAB_AMDhuJMOt1tZWRpYS5zdGVhbXBvd2VyZWQuY29t)__` |
| 27 | 193.3.190.75 | 85 | فعال | `tg://proxy?server=193.3.190.75&port=85&secret=ee0c30628212cbbd7ac519130205525d1569612e737465616d706f77657265642e636f6d` |
| 28 | 62.60.178.4 | 8888 | فعال | `tg://proxy?server=62.60.178.4&port=8888&secret=7gAA8A8Pd1VV9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 29 | 66978828877833.meli.zban-mas.info | 8888 | فعال | `tg://proxy?server=66978828877833.meli.zban-mas.info&port=8888&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 30 | 62.60.178.94 | 9741 | فعال | `tg://proxy?server=62.60.178.94&port=9741&secret=ee0000f00f0f775555fffffff5006e2e696d656469612e737465616d706f77657265642e636f6d` |


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
