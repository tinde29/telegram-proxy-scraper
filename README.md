# Telegram Proxy Scraper

[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Python](https://img.shields.io/badge/python-3.9-blue)](https://www.python.org/downloads/)
[![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/tinde29/telegram-proxy-scraper/issues)
[![Proxy Scraper Workflow](https://github.com/tinde29/telegram-proxy-scraper/actions/workflows/scraper.yml/badge.svg)](https://github.com/tinde29/telegram-proxy-scraper/actions/workflows/scraper.yml)
![GitHub last commit](https://img.shields.io/github/last-commit/tinde29/telegram-proxy-scraper)
![GitHub issues](https://img.shields.io/github/issues/tinde29/telegram-proxy-scraper)

**آخرین به‌روزرسانی پروکسی‌ها**: 25 July 2025, 13:50 UTC (به وقت ایران: 17:20)

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
| 1 | 87.248.132.36 | 70 | فعال | `tg://proxy?server=87.248.132.36&port=70&secret=eed77db43ee3721f0fcb40a4ff63b5cd276D656469612E737465616D706F77657265642E636F6D` |
| 2 | 37.27.31.197 | 443 | فعال | `tg://proxy?server=37.27.31.197&port=443&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 3 | 8443.iropt-f.ir | 443 | فعال | `tg://proxy?server=8443.iropt-f.ir&port=443&secret=eed77db43ee3721f0fcb40a4ff63b5cd276D656469612E737465616D706F77657265642E636F6D` |
| 4 | 91.99.194.27 | 47 | فعال | `tg://proxy?server=91.99.194.27&port=47&secret=7gAA8A8Pd1VV____9QBtLmlfbWVkaWEuc3RlYW0tcG93ZXJlZF8)__` |
| 5 | 00.11.22.33-44.ir | 443 | فعال | `tg://proxy?server=00.11.22.33-44.ir&port=443&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 6 | fasst.sitemcinet.co.uk | 443 | فعال | `tg://proxy?server=fasst.sitemcinet.co.uk&port=443&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t)__` |
| 7 | 157.180.80.64 | 8888 | فعال | `tg://proxy?server=157.180.80.64&port=8888&secret=FgMBAgABAAH8AwOG4kw63Q` |
| 8 | 62.60.178.115 | 443 | فعال | `tg://proxy?server=62.60.178.115&port=443&secret=1603010200010001fc030386e24c3add` |
| 9 | www.galacticfireworks.pro. | 888 | فعال | `tg://proxy?server=www.galacticfireworks.pro.&port=888&secret=ee0c30628212cbbd7ac519130205525d1569612e737465616d706f77657265642e636f6d)__` |
| 10 | 500.meli.zban-mas.info | 8888 | فعال | `tg://proxy?server=500.meli.zban-mas.info&port=8888&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 11 | ai.parsa-learning.ir. | 333 | فعال | `tg://proxy?server=ai.parsa-learning.ir.&port=333&secret=7hAQEP8PSAZT____9QBuLmlpYS5zdGVhbXBvd2VyZWQuY29t` |
| 12 | kheybar.co.uk | 443 | فعال | `tg://proxy?server=kheybar.co.uk&port=443&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 13 | 109.107.178.86 | 443000 | فعال | `tg://proxy?server=109.107.178.86&port=443000&secret=7hYDAQIAAQAH8AMDhuJMOt1tZWRpYS5zdGVhbXBvd2VyZWQuY29tbWVkaWEuc3RlYW1wb3dlcmVkLmNvbQ` |
| 14 | 157.180.75.225 | 888 | فعال | `tg://proxy?server=157.180.75.225&port=888&secret=eeNEgYdJvXrFGRMCIMJdCQ` |
| 15 | 47.250.194.92 | 443 | فعال | `tg://proxy?server=47.250.194.92&port=443&secret=ee3334dae07eee5a41de9d17eb514e4f3e617a7572652e6d6963726f736f66742e636f6d` |
| 16 | 136.243.3.109 | 443 | فعال | `tg://proxy?server=136.243.3.109&port=443&secret=FgMBAgABAAH8AwOG4kw63Q` |
| 17 | 136.243.3.109 | 443 | فعال | `tg://proxy?server=136.243.3.109&port=443&secret=1603010200010001fc030386e24c3add` |
| 18 | systemfull.gjesus.info | 443 | فعال | `tg://proxy?server=systemfull.gjesus.info&port=443&secret=ee1603010200010001fc030386e24c3add6d656469612e737465616d706f77657265642e636f6d` |
| 19 | 91.99.206.83 | 70 | فعال | `tg://proxy?server=91.99.206.83&port=70&secret=7gAA8A8Pd1VV____9QBuLmktLXcuZ28tLS0=` |
| 20 | 151.244.85.77 | 343 | فعال | `tg://proxy?server=151.244.85.77&port=343&secret=eed77db43ee3721f0fcb40a4ff63b5cd276D656469612E737465616D706F77657265642E636F6D` |
| 21 | 91.99.193.144 | 59065 | فعال | `tg://proxy?server=91.99.193.144&port=59065&secret=eed77db43ee3721f0fcb40a4ff63b5cd276D656469612E737465616D706F77657265642E636F6D` |
| 22 | 159.69.83.188 | 8080 | فعال | `tg://proxy?server=159.69.83.188&port=8080&secret=7gggggggggggggg______-4tdy5nby0=)__` |
| 23 | 157.180.83.88 | 8888 | فعال | `tg://proxy?server=157.180.83.88&port=8888&secret=FgMBAgABAAH8AwOG4kw63Q` |
| 24 | 91.99.228.230 | 59065 | فعال | `tg://proxy?server=91.99.228.230&port=59065&secret=eed77db43ee3721f0fcb40a4ff63b5cd276D656469612E737465616D706F77657265642E636F6D` |
| 25 | 151.244.85.59 | 70 | فعال | `tg://proxy?server=151.244.85.59&port=70&secret=ee0000f00f0f775555fffffff5006e2e696D656469612E737465616D706F77657265642E636F6D` |
| 26 | 87.229.100.159 | 443 | فعال | `tg://proxy?server=87.229.100.159&port=443&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 27 | 47.243.24.171 | 443 | فعال | `tg://proxy?server=47.243.24.171&port=443&secret=ee25dd09dee50fc4772bd314daee220eaf617a7572652e6d6963726f736f66742e636f6d` |
| 28 | 157.180.119.71 | 551 | فعال | `tg://proxy?server=157.180.119.71&port=551&secret=eeNEgYdJvXrFGRMCIMJdCQ` |
| 29 | 200.meli.zban-mas.info | 8888 | فعال | `tg://proxy?server=200.meli.zban-mas.info&port=8888&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 30 | 91.99.105.128 | 8888 | فعال | `tg://proxy?server=91.99.105.128&port=8888&secret=7gAA8A8Pd1VV` |


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
