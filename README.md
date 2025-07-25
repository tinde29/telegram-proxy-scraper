# Telegram Proxy Scraper

[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Python](https://img.shields.io/badge/python-3.9-blue)](https://www.python.org/downloads/)
[![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/tinde29/telegram-proxy-scraper/issues)
[![Proxy Scraper Workflow](https://github.com/tinde29/telegram-proxy-scraper/actions/workflows/scraper.yml/badge.svg)](https://github.com/tinde29/telegram-proxy-scraper/actions/workflows/scraper.yml)
![GitHub last commit](https://img.shields.io/github/last-commit/tinde29/telegram-proxy-scraper)
![GitHub issues](https://img.shields.io/github/issues/tinde29/telegram-proxy-scraper)

**آخرین به‌روزرسانی پروکسی‌ها**: 25 July 2025, 07:00 UTC (به وقت ایران: 10:30)

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
| 1 | 95.216.22.207 | 443 | فعال | `tg://proxy?server=95.216.22.207&port=443&secret=iORid5lJ237IiBMGYMQMdw` |
| 2 | 62.60.176.59 | 443 | فعال | `tg://proxy?server=62.60.176.59&port=443&secret=7hYDAQIAAQAH8AMDhuJMOt1tZWRpYS5zdGVhbXBvd2VyZWQuY29tbWVkaWEuc3RlYW1wb3dlcmVkLmNvbQ)|` |
| 3 | 157.180.47.224 | 443 | فعال | `tg://proxy?server=157.180.47.224&port=443&secret=1603010200010001fc030386e24c3add` |
| 4 | vip2.abanol1.info | 70 | فعال | `tg://proxy?server=vip2.abanol1.info&port=70&secret=7td9tD7jch8Py0Ck_2O1zSdtZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 5 | 104.21.21.77 | 443 | فعال | `tg://proxy?server=104.21.21.77&port=443&secret=3QAAAAAAAAAAAAAAAAAAAAA**` |
| 6 | 4.Ir.ir.ir.ir.ir.zban-mas.info | 8888 | فعال | `tg://proxy?server=4.Ir.ir.ir.ir.ir.zban-mas.info&port=8888&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 7 | 94.130.218.244 | 443 | فعال | `tg://proxy?server=94.130.218.244&port=443&secret=EERighJJvXrFGRMCIMJdCQ==` |
| 8 | 87.248.134.48 | 70 | فعال | `tg://proxy?server=87.248.134.48&port=70&secret=eed77db43ee3721f0fcb40a4ff63b5cd276D656469612E737465616D706F77657265642E636F6D` |
| 9 | www.hihim.sbs | 888 | فعال | `tg://proxy?server=www.hihim.sbs&port=888&secret=ee0c30628212cbbd7ac519130205525d1569612e737465616d706f77657265642e636f6d)__` |
| 10 | 78.47.82.66 | 443 | فعال | `tg://proxy?server=78.47.82.66&port=443&secret=DDBighLLvXrFGRMCBVJdFQ==` |
| 11 | 47.254.231.224 | 443 | فعال | `tg://proxy?server=47.254.231.224&port=443&secret=ee47c0ce85abd33aac10f02f06fee66ac7617a7572652e6d6963726f736f66742e636f6d` |
| 12 | ai.qwert-naser5.ir | 852 | فعال | `tg://proxy?server=ai.qwert-naser5.ir&port=852&secret=DDBighLLvXrFGRMCBVJdFQRueWVrdGFuZXQuY29tZmFyYTrhdi5jb212YZ6ubmFqXeEuY29t` |
| 13 | 188.166.49.247 | 443 | فعال | `tg://proxy?server=188.166.49.247&port=443&secret=d1d069d2fb0fca4d28cd0e53bda39bbb` |
| 14 | 172.86.66.208.irancell.ir.dijikala.co.uk | 443 | فعال | `tg://proxy?server=172.86.66.208.irancell.ir.dijikala.co.uk&port=443&secret=7hYDAQIAAfADA4biTDrd3E53d3cuZ29vZ2xlLmNvbQ==` |
| 15 | 185.117.0.153 | 8882 | فعال | `tg://proxy?server=185.117.0.153&port=8882&secret=eed700433aba3557d5e83d82beb4ab735873332e616d617a6f6e6177732e636f6d` |
| 16 | 45.129.199.72 | 443 | فعال | `tg://proxy?server=45.129.199.72&port=443&secret=ee100404ff0f48064fffffff9001b8696d696d656469612e737465616d706f77657265642e636f6d` |
| 17 | 62.60.176.38 | 443 | فعال | `tg://proxy?server=62.60.176.38&port=443&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 18 | 164.90.237.85 | 80 | فعال | `tg://proxy?server=164.90.237.85&port=80&secret=3V9HEDbXrf_pCKa76RM2stc` |
| 19 | 62.60.179.82 | 443 | فعال | `tg://proxy?server=62.60.179.82&port=443&secret=7hAQEP8PSAZT____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 20 | https.link-a1.ir | 443 | فعال | `tg://proxy?server=https.link-a1.ir&port=443&secret=eed77db43ee3721f0fcb40a4ff63b5cd276D656469612E737465616D706F77657265642E636F6D` |
| 21 | 46.249.110.54 | 443 | فعال | `tg://proxy?server=46.249.110.54&port=443&secret=15115115115115115115115115115115)|` |
| 22 | Https.iropt-j.ir | 443 | فعال | `tg://proxy?server=Https.iropt-j.ir&port=443&secret=ee07df7df7df7dfffffdfffffffffffc07646f776e6c6f61642e77696e646f77737570646174652e636f6d` |
| 23 | 91.99.99.2 | 443 | فعال | `tg://proxy?server=91.99.99.2&port=443&secret=7gD_AA___wD_9VVf______VtZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 24 | 5.35.46.6 | 443 | فعال | `tg://proxy?server=5.35.46.6&port=443&secret=eed77db43ee3721f0fcb40a4ff63b5cd276D656469612E737465616D706F77657265642E636F6D` |
| 25 | 77.238.229.198 | 710 | فعال | `tg://proxy?server=77.238.229.198&port=710&secret=eeNEgYdJvXrFGRMCIMJdCQ` |
| 26 | 14.102.10.121 | 85 | فعال | `tg://proxy?server=14.102.10.121&port=85&secret=7gD_AA_wD_9VVf____VmLmtvLS0` |
| 27 | 91.99.233.205 | 8888 | فعال | `tg://proxy?server=91.99.233.205&port=8888&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 28 | 157.180.123.236 | 8888 | فعال | `tg://proxy?server=157.180.123.236&port=8888&secret=FgMBAgABAAH8AwOG4kw63Q` |
| 29 | 7711.meli.zban-mas.info | 8888 | فعال | `tg://proxy?server=7711.meli.zban-mas.info&port=8888&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 30 | 91.99.226.187 | 155 | فعال | `tg://proxy?server=91.99.226.187&port=155&secret=7hYDAQIAAQAH8AMDhuJMOt1tZWRpYS5zdGVhbXBvd2VyZWQuY29tbWVkaWEuc3RlYW1wb3dlcmVkLmNvbQ` |


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
