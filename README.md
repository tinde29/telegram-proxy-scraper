# Telegram Proxy Scraper

[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Python](https://img.shields.io/badge/python-3.9-blue)](https://www.python.org/downloads/)
[![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/tinde29/telegram-proxy-scraper/issues)
[![Proxy Scraper Workflow](https://github.com/tinde29/telegram-proxy-scraper/actions/workflows/scraper.yml/badge.svg)](https://github.com/tinde29/telegram-proxy-scraper/actions/workflows/scraper.yml)
![GitHub last commit](https://img.shields.io/github/last-commit/tinde29/telegram-proxy-scraper)
![GitHub issues](https://img.shields.io/github/issues/tinde29/telegram-proxy-scraper)

**آخرین به‌روزرسانی پروکسی‌ها**: 24 July 2025, 03:53 UTC (به وقت ایران: 07:23)

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
| 1 | 87.248.132.177 | 200 | فعال | `tg://proxy?server=87.248.132.177&port=200&secret=ee0000f00f0f775555fffffff5006e2e69646F776E6C6F61642E77696E646F77737570646174652E636F6D` |
| 2 | 157.180.46.166 | 8888 | فعال | `tg://proxy?server=157.180.46.166&port=8888&secret=DD1603010200010001fc030386e24c3add` |
| 3 | 91.99.166.4 | 8888 | فعال | `tg://proxy?server=91.99.166.4&port=8888&secret=7gAA8A8Pd1VV////9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 4 | 140.233.187.98 | 443 | فعال | `tg://proxy?server=140.233.187.98&port=443&secret=eed77db43ee3721f0fcb40a4ff63b5cd276d656469612e737465616d706f77657265642e636f6d` |
| 5 | bib.bib.game.zx2hgujoiah-xy1xutr045-2tk.ir | 8443 | فعال | `tg://proxy?server=bib.bib.game.zx2hgujoiah-xy1xutr045-2tk.ir&port=8443&secret=7gAA8A8Pd1VV____9QBuLmktLXcuZ28tLS0=` |
| 6 | 156.253.5.208 | 443 | فعال | `tg://proxy?server=156.253.5.208&port=443&secret=0272543f50dea5f345c032ed2a438bde` |
| 7 | 151.244.50.27 | 70 | فعال | `tg://proxy?server=151.244.50.27&port=70&secret=eed77db43ee3721f0fcb40a4ff63b5cd276D656469612E737465616D706F77657265642E636F6D` |
| 8 | 91.99.129.94 | 155 | فعال | `tg://proxy?server=91.99.129.94&port=155&secret=7hYDAQIAAQAH8AMDhuJMOt1tZWRpYS5zdGVhbXBvd2VyZWQuY29tbWVkaWEuc3RlYW1wb3dlcmVkLmNvbQ` |
| 9 | 157.180.80.64 | 8888 | فعال | `tg://proxy?server=157.180.80.64&port=8888&secret=FgMBAgABAAH8AwOG4kw63Q` |
| 10 | 151.244.85.15 | 70 | فعال | `tg://proxy?server=151.244.85.15&port=70&secret=7gffffffff` |
| 11 | 89.251.10.20 | 443 | فعال | `tg://proxy?server=89.251.10.20&port=443&secret=ee151151151151151151151151151151156d656469612e737465616d706f77657265642e636f6d)[پروکسی](https://t.me/proxy?server=89.251.10.20` |
| 12 | 500.meli.zban-mas.info | 8888 | فعال | `tg://proxy?server=500.meli.zban-mas.info&port=8888&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 13 | 49.12.7.170 | 155 | فعال | `tg://proxy?server=49.12.7.170&port=155&secret=dd1603010200010001fc030386e24c3add` |
| 14 | 91.99.172.214 | 8888 | فعال | `tg://proxy?server=91.99.172.214&port=8888&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 15 | 79.172.228.84 | 70 | فعال | `tg://proxy?server=79.172.228.84&port=70&secret=ee0000f00f0f775555fffffff5006e2e696D656469612E737465616D706F77657265642E636F6D)|[پروکسی](https://t.me/proxy?server=79.172.228.201` |
| 16 | 195.201.58.218 | 155 | فعال | `tg://proxy?server=195.201.58.218&port=155&secret=ee0000f00f0f775555fffffff5006e2e696d656469612e737465616d706f77657265642e636f6d` |
| 17 | 62.60.178.119 | 443 | فعال | `tg://proxy?server=62.60.178.119&port=443&secret=7hYDAQIAAQAH8AMDhuJMOt1tZWRpYS5zdGVhbXBvd2VyZWQuY29tbWVkaWEuc3RlYW1wb3dlcmVkLmNvbQ)`` |
| 18 | 91.99.152.221 | 443 | فعال | `tg://proxy?server=91.99.152.221&port=443&secret=eee6607B90889CC60719D2170CB2851962737465616D706F77657265642E636F6D` |
| 19 | 157.180.126.9 | 8888 | فعال | `tg://proxy?server=157.180.126.9&port=8888&secret=1603010200010001fc030386e24c3add` |
| 20 | 45.93.170.26 | 3389 | فعال | `tg://proxy?server=45.93.170.26&port=3389&secret=eeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeee31302e31302e33342e3336` |
| 21 | 157.180.93.115 | 443 | فعال | `tg://proxy?server=157.180.93.115&port=443&secret=iORid5lJ237IiBMGYMQMdw` |
| 22 | 62.60.179.43 | 443 | فعال | `tg://proxy?server=62.60.179.43&port=443&secret=7hAQEP8PSAZT____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 23 | fasst.sitemcinet.co.uk | 443 | فعال | `tg://proxy?server=fasst.sitemcinet.co.uk&port=443&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 24 | my.parsa-learning.ir. | 443 | فعال | `tg://proxy?server=my.parsa-learning.ir.&port=443&secret=7hAQEP8PSAZT____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t)__` |
| 25 | 62.60.177.174 | 8443 | فعال | `tg://proxy?server=62.60.177.174&port=8443&secret=FgMBAgABAAfwAwOG4kw63Q` |
| 26 | 91.99.146.38 | 888 | فعال | `tg://proxy?server=91.99.146.38&port=888&secret=7gwwYoISy716xRkTAgVSXRVpYS5zdGVhbXBvd2VyZWQuY29t` |
| 27 | halftime.parsintalk.ir | 443 | فعال | `tg://proxy?server=halftime.parsintalk.ir&port=443&secret=7hYDAQIAAQAB_AMDhuJMOt1tZWRpYS5zdGVhbXBvd2VyZWQuY29t)__` |
| 28 | 7.248.132.96 | 200 | فعال | `tg://proxy?server=7.248.132.96&port=200&secret=eed77db43ee3721f0fcb40a4ff63b5cd276D656469612E737465616D706F77657265642E636F6D` |
| 29 | Yoast.harcibasheokeye.ir | 918 | فعال | `tg://proxy?server=Yoast.harcibasheokeye.ir&port=918&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t)__` |
| 30 | 111.Ir.ir.ir.ir.ir.zban-mas.info | 8888 | فعال | `tg://proxy?server=111.Ir.ir.ir.ir.ir.zban-mas.info&port=8888&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |


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
