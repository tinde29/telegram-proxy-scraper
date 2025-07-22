# Telegram Proxy Scraper

[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Python](https://img.shields.io/badge/python-3.9-blue)](https://www.python.org/downloads/)
[![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/tinde29/telegram-proxy-scraper/issues)
[![Proxy Scraper Workflow](https://github.com/tinde29/telegram-proxy-scraper/actions/workflows/scraper.yml/badge.svg)](https://github.com/tinde29/telegram-proxy-scraper/actions/workflows/scraper.yml)
![GitHub last commit](https://img.shields.io/github/last-commit/tinde29/telegram-proxy-scraper)
![GitHub issues](https://img.shields.io/github/issues/tinde29/telegram-proxy-scraper)

**آخرین به‌روزرسانی پروکسی‌ها**: 22 July 2025, 13:52 UTC (به وقت ایران: 17:22)

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
| 1 | leveldaemi.fiziotr.info | 443 | فعال | `tg://proxy?server=leveldaemi.fiziotr.info&port=443&secret=7hYDAQIAAQAB_AMDhuJMOt1tZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 2 | 89.116.246.201 | 443 | فعال | `tg://proxy?server=89.116.246.201&port=443&secret=dd146231426d22b827d0f764cbe6f61956` |
| 3 | 91.99.175.203 | 8888 | فعال | `tg://proxy?server=91.99.175.203&port=8888&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 4 | 5.meli.meli.zban-mas.info | 8888 | فعال | `tg://proxy?server=5.meli.meli.zban-mas.info&port=8888&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t)__` |
| 5 | vip.bomberoo.co.uk | 155 | فعال | `tg://proxy?server=vip.bomberoo.co.uk&port=155&secret=7hYDAQIAAQAH8AMDhuJMOt1tZWRpYS5zdGVhbXBvd2VyZWQuY29tbWVkaWEuc3RlYW1wb3dlcmVkLmNvbQ)|` |
| 6 | 157.180.122.194 | 551 | فعال | `tg://proxy?server=157.180.122.194&port=551&secret=eeNEgYdJvXrFGRMCIMJdCQ` |
| 7 | 65.108.12.153 | 65 | فعال | `tg://proxy?server=65.108.12.153&port=65&secret=1320PuNyHw_LQKT_Y7XNJw` |
| 8 | 46.249.110.245 | 9741 | فعال | `tg://proxy?server=46.249.110.245&port=9741&secret=ee0000f00f0f775555fffffff5006e2e696D656469612E737465616D706F77657265642E636F6D` |
| 9 | 157.180.84.199 | 888 | فعال | `tg://proxy?server=157.180.84.199&port=888&secret=eeNEgYdJvXrFGRMCIMJdCQ` |
| 10 | 140.233.187.60 | 443 | فعال | `tg://proxy?server=140.233.187.60&port=443&secret=eed77db43ee3721f0fcb40a4ff63b5cd276d656469612e737465616d706f77657265642e636f6d` |
| 11 | 62.60.178.119 | 443 | فعال | `tg://proxy?server=62.60.178.119&port=443&secret=7hYDAQIAAQAH8AMDhuJMOt1tZWRpYS5zdGVhbXBvd2VyZWQuY29tbWVkaWEuc3RlYW1wb3dlcmVkLmNvbQ` |
| 12 | 51.38.223.137 | 110 | فعال | `tg://proxy?server=51.38.223.137&port=110&secret=ee050e992bf52dd097871abc372c25dede7777772e636c6f7564666c6172652e636f6d)|` |
| 13 | 83.172.153.226 | 85 | فعال | `tg://proxy?server=83.172.153.226&port=85&secret=dd306cb73bd735551ca3b59f32e05b45e9` |
| 14 | 31.58.134.32 | 8888 | فعال | `tg://proxy?server=31.58.134.32&port=8888&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 15 | 185.95.159.231 | 9741 | فعال | `tg://proxy?server=185.95.159.231&port=9741&secret=ee0000f00f0f775555fffffff5006e2e696d656469612e737465616d706f77657265642e636f6d` |
| 16 | 4468855.meli.zban-mas.info | 8888 | فعال | `tg://proxy?server=4468855.meli.zban-mas.info&port=8888&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 17 | 99955.meli.zban-mas.info | 8888 | فعال | `tg://proxy?server=99955.meli.zban-mas.info&port=8888&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 18 | 204.76.203.84 | 443 | فعال | `tg://proxy?server=204.76.203.84&port=443&secret=15115115115115115115115115115115` |
| 19 | 157.180.120.10 | 8888 | فعال | `tg://proxy?server=157.180.120.10&port=8888&secret=FgMBAgABAAH8AwOG4kw63Q` |
| 20 | 62.60.178.2 | 8888 | فعال | `tg://proxy?server=62.60.178.2&port=8888&secret=7gAA8A8Pd1VV9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t____` |
| 21 | 23.236.186.146 | 443 | فعال | `tg://proxy?server=23.236.186.146&port=443&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 22 | 87.248.132.42 | 200 | فعال | `tg://proxy?server=87.248.132.42&port=200&secret=eeNEgYdJvXrFGRMCIMJdCQ)`` |
| 23 | 157.180.61.201 | 1080 | فعال | `tg://proxy?server=157.180.61.201&port=1080&secret=1320PuNyHw_LQKT_Y7XNJw` |
| 24 | 91.99.237.104 | 8888 | فعال | `tg://proxy?server=91.99.237.104&port=8888&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 25 | 103.161.35.45 | 155 | فعال | `tg://proxy?server=103.161.35.45&port=155&secret=ee1aa5c80106b768b926cf330d71eb95bc6d656469612e737465616d706f77657265642e636f6d**` |
| 26 | 89.251.10.21 | 443 | فعال | `tg://proxy?server=89.251.10.21&port=443&secret=ee151151151151151151151151151151156d656469612e737465616d706f77657265642e636f6d)__` |
| 27 | 87.248.132.199 | 200 | فعال | `tg://proxy?server=87.248.132.199&port=200&secret=7gAA8A8Pd1VV____9QBuLmktLXcuZ28tLS0=` |
| 28 | 4.meli.zban-mas.info | 8888 | فعال | `tg://proxy?server=4.meli.zban-mas.info&port=8888&secret=7gAA8A8Pd1VV////9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 29 | 8.217.25.47 | 443 | فعال | `tg://proxy?server=8.217.25.47&port=443&secret=ee52b986ec192f5e0d25d7e2ee6fdeffcc617a7572652e6d6963726f736f66742e636f6d` |
| 30 | 88.210.10.165 | 443000 | فعال | `tg://proxy?server=88.210.10.165&port=443000&secret=7hYDAQIAAQAH8AMDhuJMOt1tZWRpYS5zdGVhbXBvd2VyZWQuY29tbWVkaWEuc3RlYW1wb3dlcmVkLmNvbQ` |


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
