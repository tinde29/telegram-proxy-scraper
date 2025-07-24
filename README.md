# Telegram Proxy Scraper

[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Python](https://img.shields.io/badge/python-3.9-blue)](https://www.python.org/downloads/)
[![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/tinde29/telegram-proxy-scraper/issues)
[![Proxy Scraper Workflow](https://github.com/tinde29/telegram-proxy-scraper/actions/workflows/scraper.yml/badge.svg)](https://github.com/tinde29/telegram-proxy-scraper/actions/workflows/scraper.yml)
![GitHub last commit](https://img.shields.io/github/last-commit/tinde29/telegram-proxy-scraper)
![GitHub issues](https://img.shields.io/github/issues/tinde29/telegram-proxy-scraper)

**آخرین به‌روزرسانی پروکسی‌ها**: 24 July 2025, 07:00 UTC (به وقت ایران: 10:30)

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
| 1 | 157.180.30.251 | 443 | فعال | `tg://proxy?server=157.180.30.251&port=443&secret=iORid5lJ237IiBMGYMQMdw==` |
| 2 | 488.ir.ir.ir.ir.ir.zban-mas.info | 8888 | فعال | `tg://proxy?server=488.ir.ir.ir.ir.ir.zban-mas.info&port=8888&secret=7gAA8A8Pd1VV__9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 3 | 193.3.190.70 | 85 | فعال | `tg://proxy?server=193.3.190.70&port=85&secret=ee0000f00f0f775555fffffff5006e2e696d656469612e737465616d706f77657265642e636f6d` |
| 4 | 91.99.150.26 | 443 | فعال | `tg://proxy?server=91.99.150.26&port=443&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t)**` |
| 5 | 7.meli.meli.zban-mas.info | 8888 | فعال | `tg://proxy?server=7.meli.meli.zban-mas.info&port=8888&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t)__` |
| 6 | mtproxy10.alphacyber.org | 443 | فعال | `tg://proxy?server=mtproxy10.alphacyber.org&port=443&secret=dde5ceff7c8a4a80fcad3dae7d23f3ac65` |
| 7 | 87.248.134.37 | 70 | فعال | `tg://proxy?server=87.248.134.37&port=70&secret=eed77db43ee3721f0fcb40a4ff63b5cd276D656469612E737465616D706F77657265642E636F6D` |
| 8 | 62.112.221.49 | 1122 | فعال | `tg://proxy?server=62.112.221.49&port=1122&secret=d3dc6819743ceae6a8871ce5cb04ca33` |
| 9 | 13.meli.zban-mas.info | 8888 | فعال | `tg://proxy?server=13.meli.zban-mas.info&port=8888&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t)__` |
| 10 | 10.Ir.ir.ir.ir.ir.zban-mas.info | 8888 | فعال | `tg://proxy?server=10.Ir.ir.ir.ir.ir.zban-mas.info&port=8888&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 11 | 57.129.92.216 | 70 | فعال | `tg://proxy?server=57.129.92.216&port=70&secret=eeb7faf1ae6383bae0bdc3c4289759ce426d656469612e737465616d706f77657265642e636f6d` |
| 12 | 93.88.205.5 | 888 | فعال | `tg://proxy?server=93.88.205.5&port=888&secret=eeNEgYdJvXrFGRMCIMJdCQ` |
| 13 | 93.88.205.37 | 85 | فعال | `tg://proxy?server=93.88.205.37&port=85&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 14 | 45.135.192.245 | 85 | فعال | `tg://proxy?server=45.135.192.245&port=85&secret=ee0000f00f0f775555fffffff5006e2e69646F776E6C6F61642E77696E646F77737570646174652E636F6D` |
| 15 | 88.99.61.188 | 2908 | فعال | `tg://proxy?server=88.99.61.188&port=2908&secret=DDBighLLvXrFGRMCBVJdFQRueWVrdGFuZXQuY29t` |
| 16 | 518.8-58-185.ir | 443 | فعال | `tg://proxy?server=518.8-58-185.ir&port=443&secret=1320PuNyHw_LQKT_Y7XNJw==` |
| 17 | 195.201.58.218 | 155 | فعال | `tg://proxy?server=195.201.58.218&port=155&secret=ee0000f00f0f775555fffffff5006e2e696d656469612e737465616d706f77657265642e636f6d` |
| 18 | 62.60.178.185 | 443 | فعال | `tg://proxy?server=62.60.178.185&port=443&secret=7hYDAQIAAQAH8AMDhuJMOt1tZWRpYS5zdGVhbXBvd2VyZWQuY29tbWVkaWEuc3RlYW1wb3dlcmVkLmNvbQ` |
| 19 | 91.107.168.188 | 27 | فعال | `tg://proxy?server=91.107.168.188&port=27&secret=1320PuNyHw_LQKT_Y7XNJw==` |
| 20 | 89.110.78.179 | 443 | فعال | `tg://proxy?server=89.110.78.179&port=443&secret=ee07df7df7df7dfffffdfffffffffffc07646f776e6c6f61642e77696e646f77737570646174652e636f6d` |
| 21 | 193.3.190.74 | 85 | فعال | `tg://proxy?server=193.3.190.74&port=85&secret=ee0c30628212cbbd7ac519130205525d1569612e737465616d706f77657265642e636f6d` |
| 22 | 91.99.80.236 | 443 | فعال | `tg://proxy?server=91.99.80.236&port=443&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 23 | 89.116.246.201 | 443 | فعال | `tg://proxy?server=89.116.246.201&port=443&secret=146231426d22b827d0f764cbe6f61956` |
| 24 | 49.12.38.200 | 155 | فعال | `tg://proxy?server=49.12.38.200&port=155&secret=dd1603010200010001fc030386e24c3add|[پروکسی](tg://proxy?server=62.60.178.253` |
| 25 | 87.248.132.70 | 155 | فعال | `tg://proxy?server=87.248.132.70&port=155&secret=ee0000f00f0f775555fffffff5006e2e69646f776e6c6f61642e77696e646f77737570646174652e636f6d` |
| 26 | 62.60.177.109 | 443 | فعال | `tg://proxy?server=62.60.177.109&port=443&secret=7hYDAQIAAQAH8AMDhuJMOt1tZWRpYS5zdGVhbXBvd2VyZWQuY29tbWVkaWEuc3RlYW1wb3dlcmVkLmNvbQ` |
| 27 | 00800.meli.zban-mas.info | 8888 | فعال | `tg://proxy?server=00800.meli.zban-mas.info&port=8888&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t**` |
| 28 | 62.60.179.65 | 443 | فعال | `tg://proxy?server=62.60.179.65&port=443&secret=7hAQEP8PSAZT____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 29 | 87.248.132.55 | 200 | فعال | `tg://proxy?server=87.248.132.55&port=200&secret=79e344818749bd7ac519130220c25d09` |
| 30 | 164.90.237.85 | 80 | فعال | `tg://proxy?server=164.90.237.85&port=80&secret=3V9HEDbXrf_pCKa76RM2stc` |


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
