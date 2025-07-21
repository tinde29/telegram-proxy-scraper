# Telegram Proxy Scraper

[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Python](https://img.shields.io/badge/python-3.9-blue)](https://www.python.org/downloads/)
[![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/tinde29/telegram-proxy-scraper/issues)
[![Proxy Scraper Workflow](https://github.com/tinde29/telegram-proxy-scraper/actions/workflows/scraper.yml/badge.svg)](https://github.com/tinde29/telegram-proxy-scraper/actions/workflows/scraper.yml)
![GitHub last commit](https://img.shields.io/github/last-commit/tinde29/telegram-proxy-scraper)
![GitHub issues](https://img.shields.io/github/issues/tinde29/telegram-proxy-scraper)

**آخرین به‌روزرسانی پروکسی‌ها**: 21 July 2025, 14:12 UTC (به وقت ایران: 17:42)

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
| 1 | cai7kkj46fbf.dop1000.com | 443 | فعال | `tg://proxy?server=cai7kkj46fbf.dop1000.com&port=443&secret=ee21ef372ec7034a96b00807b1ed45d42d636c7562686f7573652e7075626e75622e636f6d` |
| 2 | 79.172.228.10 | 700 | فعال | `tg://proxy?server=79.172.228.10&port=700&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 3 | 157.90.162.107 | 8888 | فعال | `tg://proxy?server=157.90.162.107&port=8888&secret=FgMBAgABAAH8AwOG4kw63Q` |
| 4 | 87.248.132.33 | 200 | فعال | `tg://proxy?server=87.248.132.33&port=200&secret=eed77db43ee3721f0fcb40a4ff63b5cd276D656469612E737465616D706F77657265642E636F6D` |
| 5 | newdomain1.co.uk | 443 | فعال | `tg://proxy?server=newdomain1.co.uk&port=443&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 6 | 78.40.193.73 | 8888 | فعال | `tg://proxy?server=78.40.193.73&port=8888&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 7 | 87.248.134.37 | 70 | فعال | `tg://proxy?server=87.248.134.37&port=70&secret=eed77db43ee3721f0fcb40a4ff63b5cd276D656469612E737465616D706F77657265642E636F6D)__` |
| 8 | markino.xyz | 443 | فعال | `tg://proxy?server=markino.xyz&port=443&secret=ee320658d3147dad619606da05bcc1f49173332e616d617a6f6e6177732e636f6d` |
| 9 | 188.166.101.248 | 85 | فعال | `tg://proxy?server=188.166.101.248&port=85&secret=DDBighLLvXrFGRMCBVJdFQ==` |
| 10 | 62.60.179.158 | 9741 | فعال | `tg://proxy?server=62.60.179.158&port=9741&secret=ee0000f00f0f775555fffffff5006e2e696d656469612e737465616d706f77657265642e636f6d` |
| 11 | 62.60.176.58 | 443 | فعال | `tg://proxy?server=62.60.176.58&port=443&secret=7hYDAQIAAQAH8AMDhuJMOt1tZWRpYS5zdGVhbXBvd2VyZWQuY29tbWVkaWEuc3RlYW1wb3dlcmVkLmNvbQ)|` |
| 12 | 95.217.77.168 | 443 | فعال | `tg://proxy?server=95.217.77.168&port=443&secret=iORid5lJ237IiBMGYMQMdw` |
| 13 | 94.130.218.244 | 443 | فعال | `tg://proxy?server=94.130.218.244&port=443&secret=104462821249bd7ac519130220c25d09` |
| 14 | www.sshputty.icu. | 888 | فعال | `tg://proxy?server=www.sshputty.icu.&port=888&secret=ee0c30628212cbbd7ac519130205525d1569612e737465616d706f77657265642e636f6d****` |
| 15 | 79.172.228.82 | 70 | فعال | `tg://proxy?server=79.172.228.82&port=70&secret=ee0000f00f0f775555fffffff5006e2e696D656469612E737465616D706F77657265642E636F6D|[پروکسی](https://t.me/proxy?server=79.172.228.201` |
| 16 | mtp.vnf.one | 11042 | فعال | `tg://proxy?server=mtp.vnf.one&port=11042&secret=dd11041104110411041104110411041104` |
| 17 | 77.246.107.227 | 70 | فعال | `tg://proxy?server=77.246.107.227&port=70&secret=ee0000f00f0f775555fffffff5006e2e696D656469612E737465616D706F77657265642E636F6D` |
| 18 | 88.99.251.22 | 443 | فعال | `tg://proxy?server=88.99.251.22&port=443&secret=104462821249bd7ac519130220c25d09` |
| 19 | 88.119.165.95 | 155 | فعال | `tg://proxy?server=88.119.165.95&port=155&secret=7s7477TTTTTTETTTTTTTtrYtRi5rby0` |
| 20 | HAMRAH-AVAL.new-visioncity.ir. | 9741 | فعال | `tg://proxy?server=HAMRAH-AVAL.new-visioncity.ir.&port=9741&secret=ee0000f00f0f775555fffffff5006e2e696d656469612e737465616d706f77657265642e636f6d` |
| 21 | 99900.meli.zban-mas.info | 8888 | فعال | `tg://proxy?server=99900.meli.zban-mas.info&port=8888&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 22 | 62.60.178.195 | 443 | فعال | `tg://proxy?server=62.60.178.195&port=443&secret=7hYDAQIAAQAH8AMDhuJMOt1tZWRpYS5zdGVhbXBvd2VyZWQuY29tbWVkaWEuc3RlYW1wb3dlcmVkLmNvbQ)|` |
| 23 | 62.60.177.165 | 8443 | فعال | `tg://proxy?server=62.60.177.165&port=8443&secret=FgMBAgABAAfwAwOG4kw63Q` |
| 24 | 146.103.97.75 | 8888 | فعال | `tg://proxy?server=146.103.97.75&port=8888&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 25 | 65.108.12.153 | 65 | فعال | `tg://proxy?server=65.108.12.153&port=65&secret=d77db43ee3721f0fcb40a4ff63b5cd27` |
| 26 | Berke.Wikimoon.sale | 443 | فعال | `tg://proxy?server=Berke.Wikimoon.sale&port=443&secret=7jK5IN_7UWQwKOL2uHjU6sFkbXl3ZWIuY2xvdWRmcm9udC5uZXQ](https://t.me/proxy?server=Startup-active.custome-tobano.avadox-zhoan.info` |
| 27 | 78.47.198.31 | 443 | فعال | `tg://proxy?server=78.47.198.31&port=443&secret=DDBighLLvXrFGRMCBVJdFQ==` |
| 28 | sell.erade60.ir | 443 | فعال | `tg://proxy?server=sell.erade60.ir&port=443&secret=eec862057ba49a7ecdf0ad4eb44cd5bb11646f776e6c6f61642e77696e646f77737570646174652e636f6d` |
| 29 | 9891.Ir.ir.ir.ir.ir.zban-mas.info | 8888 | فعال | `tg://proxy?server=9891.Ir.ir.ir.ir.ir.zban-mas.info&port=8888&secret=7gAA8A8Pd1VV9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t__` |
| 30 | 109.104.154.250 | 443 | فعال | `tg://proxy?server=109.104.154.250&port=443&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |


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
