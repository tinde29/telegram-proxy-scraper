# Telegram Proxy Scraper

[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Python](https://img.shields.io/badge/python-3.9-blue)](https://www.python.org/downloads/)
[![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/tinde29/telegram-proxy-scraper/issues)
[![Proxy Scraper Workflow](https://github.com/tinde29/telegram-proxy-scraper/actions/workflows/scraper.yml/badge.svg)](https://github.com/tinde29/telegram-proxy-scraper/actions/workflows/scraper.yml)
![GitHub last commit](https://img.shields.io/github/last-commit/tinde29/telegram-proxy-scraper)
![GitHub issues](https://img.shields.io/github/issues/tinde29/telegram-proxy-scraper)

**آخرین به‌روزرسانی پروکسی‌ها**: 24 July 2025, 13:52 UTC (به وقت ایران: 17:22)

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
| 1 | 46.62.141.211 | 8888 | فعال | `tg://proxy?server=46.62.141.211&port=8888&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 2 | 62.60.178.218 | 8080 | فعال | `tg://proxy?server=62.60.178.218&port=8080&secret=ee0000f00f0f775555fffffff5006e2e696d656469612e737465616d706f77657265642e636f6d` |
| 3 | 95.142.45.42 | 443 | فعال | `tg://proxy?server=95.142.45.42&port=443&secret=eed77db43ee3721f0fcb40a4ff63b5cd276D656469612E737465616D706F77657265642E636F6D` |
| 4 | 151.244.85.69 | 70 | فعال | `tg://proxy?server=151.244.85.69&port=70&secret=ee0000f00f0f775555fffffff5006e2e696D656469612E737465616D706F77657265642E636F6D` |
| 5 | 62.60.176.63 | 443 | فعال | `tg://proxy?server=62.60.176.63&port=443&secret=7hYDAQIAAQAH8AMDhuJMOt1tZWRpYS5zdGVhbXBvd2VyZWQuY29tbWVkaWEuc3RlYW1wb3dlcmVkLmNvbQ)__` |
| 6 | 62.60.177.113 | 343 | فعال | `tg://proxy?server=62.60.177.113&port=343&secret=FgMBAgABAAfwAwOG4kw63Q` |
| 7 | ae.mohs1736.sbs | 4637 | فعال | `tg://proxy?server=ae.mohs1736.sbs&port=4637&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 8 | 62.60.179.210 | 9741 | فعال | `tg://proxy?server=62.60.179.210&port=9741&secret=ee0000f00f0f775555fffffff5006e2e696d656469612e737465616d706f77657265642e636f6d` |
| 9 | 79.172.228.53 | 70 | فعال | `tg://proxy?server=79.172.228.53&port=70&secret=eed77db43ee3721f0fcb40a4ff63b5cd276D656469612E737465616D706F77657265642E636F6D` |
| 10 | 185.117.0.134 | 8882 | فعال | `tg://proxy?server=185.117.0.134&port=8882&secret=eed700433aba3557d5e83d82beb4ab735873332e616d617a6f6e6177732e636f6d` |
| 11 | 103.161.34.233 | 85 | فعال | `tg://proxy?server=103.161.34.233&port=85&secret=ee0000f00f0f775555fffffff5006e2e69646F776E6C6F61642E77696E646F77737570646174652E636F6D` |
| 12 | 37.27.217.240 | 155 | فعال | `tg://proxy?server=37.27.217.240&port=155&secret=ee07df7df7df7dffdffc07646f776e6c6f61642e77696e646f77737570646174652e636f6d` |
| 13 | 2.meli.meli.zban-mas.info | 8888 | فعال | `tg://proxy?server=2.meli.meli.zban-mas.info&port=8888&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t)__` |
| 14 | 89.110.90.23 | 443 | فعال | `tg://proxy?server=89.110.90.23&port=443&secret=eed77db43ee3721f0fcb40a4ff63b5cd276D656469612E737465616D706F77657265642E636F6D` |
| 15 | Cloud.irpower-g.ir | 443 | فعال | `tg://proxy?server=Cloud.irpower-g.ir&port=443&secret=eed77db43ee3721f0fcb40a4ff63b5cd276d656469612e737465616d706f77657265642e636f6d` |
| 16 | 87.248.134.42 | 200 | فعال | `tg://proxy?server=87.248.134.42&port=200&secret=eeNEgYdJvXrFGRMCIMJdCQ)__` |
| 17 | dns.parsa-learning.ir. | 333 | فعال | `tg://proxy?server=dns.parsa-learning.ir.&port=333&secret=7hAQEP8PSAZT____9QBuLmlpYS5zdGVhbXBvd2VyZWQuY29t)__` |
| 18 | iran.zibayi.shop. | 888 | فعال | `tg://proxy?server=iran.zibayi.shop.&port=888&secret=7gwwYoISy716xRkTAgVSXRVpYS5zdGVhbXBvd2VyZWQuY29t` |
| 19 | 94.130.109.131 | 155 | فعال | `tg://proxy?server=94.130.109.131&port=155&secret=ee07df7df7df7dffdffc07646f776e6c6f61642e77696e646f77737570646174652e636f6d` |
| 20 | 193.3.190.10 | 85 | فعال | `tg://proxy?server=193.3.190.10&port=85&secret=ee0000f00f0f775555fffffff5006e2e696e616d6176612e6972` |
| 21 | 77.248.132.96 | 200 | فعال | `tg://proxy?server=77.248.132.96&port=200&secret=eed77db43ee3721f0fcb40a4ff63b5cd276D656469612E737465616D706F77657265642E636F6D` |
| 22 | 94.130.218.244 | 443 | فعال | `tg://proxy?server=94.130.218.244&port=443&secret=EERighJJvXrFGRMCIMJdCQ` |
| 23 | SIGNAL.irpower-b.ir | 443 | فعال | `tg://proxy?server=SIGNAL.irpower-b.ir&port=443&secret=eed77db43ee3721f0fcb40a4ff63b5cd276D656469612E737465616D706F77657265642E636F6D` |
| 24 | 91.99.194.159 | 443 | فعال | `tg://proxy?server=91.99.194.159&port=443&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 25 | 91.99.160.52 | 443 | فعال | `tg://proxy?server=91.99.160.52&port=443&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 26 | 94.130.218.244 | 443 | فعال | `tg://proxy?server=94.130.218.244&port=443&secret=104462821249bd7ac519130220c25d09` |
| 27 | 117.55.203.133 | 56068 | فعال | `tg://proxy?server=117.55.203.133&port=56068&secret=eed77db43ee3721f0fcb40a4ff63b5cd276d656469612e737465616d706f77657265642e636f6d` |
| 28 | 193.3.190.50 | 85 | فعال | `tg://proxy?server=193.3.190.50&port=85&secret=7gAA8A8Pd1VV____9QBuLmljaGF0Z3B0LmNvbQ` |
| 29 | 88.99.149.121 | 8423 | فعال | `tg://proxy?server=88.99.149.121&port=8423&secret=DDBighLLvXrFGRMCBVJdFQRueWVrdGFuZXQuY29t` |
| 30 | 65.108.219.52 | 551 | فعال | `tg://proxy?server=65.108.219.52&port=551&secret=eeNEgYdJvXrFGRMCIMJdCQ` |


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
