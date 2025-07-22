# Telegram Proxy Scraper

[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Python](https://img.shields.io/badge/python-3.9-blue)](https://www.python.org/downloads/)
[![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/tinde29/telegram-proxy-scraper/issues)
[![Proxy Scraper Workflow](https://github.com/tinde29/telegram-proxy-scraper/actions/workflows/scraper.yml/badge.svg)](https://github.com/tinde29/telegram-proxy-scraper/actions/workflows/scraper.yml)
![GitHub last commit](https://img.shields.io/github/last-commit/tinde29/telegram-proxy-scraper)
![GitHub issues](https://img.shields.io/github/issues/tinde29/telegram-proxy-scraper)

**آخرین به‌روزرسانی پروکسی‌ها**: 22 July 2025, 06:59 UTC (به وقت ایران: 10:29)

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
| 1 | BodoBodo.khoshghovar.online. | 888 | فعال | `tg://proxy?server=BodoBodo.khoshghovar.online.&port=888&secret=ee0c30628212cbbd7ac519130205525d1569612e737465616d706f77657265642e636f6d****` |
| 2 | 78884.ir.ir.ir.ir.ir.zban-mas.info | 8888 | فعال | `tg://proxy?server=78884.ir.ir.ir.ir.ir.zban-mas.info&port=8888&secret=7gAA8A8Pd1VV9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 3 | 488.ir.ir.ir.ir.ir.zban-mas.info | 8888 | فعال | `tg://proxy?server=488.ir.ir.ir.ir.ir.zban-mas.info&port=8888&secret=7gAA8A8Pd1VV__9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 4 | 157.180.93.115 | 443 | فعال | `tg://proxy?server=157.180.93.115&port=443&secret=iORid5lJ237IiBMGYMQMdw==` |
| 5 | 91.99.105.128 | 8888 | فعال | `tg://proxy?server=91.99.105.128&port=8888&secret=7gAA8A8Pd1VV` |
| 6 | 157.180.124.237 | 8888 | فعال | `tg://proxy?server=157.180.124.237&port=8888&secret=FgMBAgABAAH8AwOG4kw63` |
| 7 | 157.180.112.134 | 8888 | فعال | `tg://proxy?server=157.180.112.134&port=8888&secret=FgMBAgABAAH8AwOG4kw63Q` |
| 8 | 91.99.100.55 | 155 | فعال | `tg://proxy?server=91.99.100.55&port=155&secret=ddec742282124f04d318551341ead76457` |
| 9 | 151.244.42.19 | 85 | فعال | `tg://proxy?server=151.244.42.19&port=85&secret=ee0000f00f0f775555fffffff5006e2e696d656469612e737465616d706f77657265642e636f6d` |
| 10 | 62.60.177.121 | 343 | فعال | `tg://proxy?server=62.60.177.121&port=343&secret=FgMBAgABAAfwAwOG4kw63Q` |
| 11 | 62.60.179.198 | 343 | فعال | `tg://proxy?server=62.60.179.198&port=343&secret=FgMBAgABAAfwAwOG4kw63Q` |
| 12 | 62.60.178.218 | 8080 | فعال | `tg://proxy?server=62.60.178.218&port=8080&secret=ee0000f00f0f775555fffffff5006e2e696d656469612e737465616d706f77657265642e636f6d` |
| 13 | 157.180.118.58 | 551 | فعال | `tg://proxy?server=157.180.118.58&port=551&secret=eeNEgYdJvXrFGRMCIMJdCQ` |
| 14 | 91.99.201.44 | 443 | فعال | `tg://proxy?server=91.99.201.44&port=443&secret=eec862057ba49a7ecdf0ad4eb44cd5bb11646f776e6c6f61642e77696e646f77737570646174652e636f6d` |
| 15 | 89.251.10.20 | 443 | فعال | `tg://proxy?server=89.251.10.20&port=443&secret=ee151151151151151151151151151151156d656469612e737465616d706f77657265642e636f6d)[پروکسی](https://t.me/proxy?server=89.251.10.20` |
| 16 | 99955.meli.zban-mas.info | 8888 | فعال | `tg://proxy?server=99955.meli.zban-mas.info&port=8888&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 17 | 62.60.177.78 | 443 | فعال | `tg://proxy?server=62.60.177.78&port=443&secret=eed77db43ee3721f0fcb40a4ff63b5cd276D656469612E737465616D706F77657265642E636F6D` |
| 18 | 91.99.175.114 | 8888 | فعال | `tg://proxy?server=91.99.175.114&port=8888&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 19 | 1.meli.zban-mas.info | 8888 | فعال | `tg://proxy?server=1.meli.zban-mas.info&port=8888&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 20 | focos-mokos.berlino-landcvixo.yokohama-1borino.eromatic.ps-fifaei.ir | 70 | فعال | `tg://proxy?server=focos-mokos.berlino-landcvixo.yokohama-1borino.eromatic.ps-fifaei.ir&port=70&secret=eed77db43ee3721f0fcb40a4ff63b5cd276d656469612e737465616d706f77657265642e636f6d)__` |
| 21 | 88.248.132.18 | 85 | فعال | `tg://proxy?server=88.248.132.18&port=85&secret=7gAA8A8Pd1VV____9QBuLmlkb3dubG9hZC53aW5kb3dzdXBkYXRlLmNvbQ` |
| 22 | 128.140.67.68 | 53246 | فعال | `tg://proxy?server=128.140.67.68&port=53246&secret=1320PuNyHw_LQKT_Y7XNJw==` |
| 23 | 93.88.205.27 | 888 | فعال | `tg://proxy?server=93.88.205.27&port=888&secret=eeNEgYdJvXrFGRMCIMJdCQ` |
| 24 | 91.201.115.102 | 443000 | فعال | `tg://proxy?server=91.201.115.102&port=443000&secret=7hYDAQIAAQAH8AMDhuJMOt1tZWRpYS5zdGVhbXBvd2VyZWQuY29tbWVkaWEuc3RlYW1wb3dlcmVkLmNvbQ` |
| 25 | 91.99.138.108 | 155 | فعال | `tg://proxy?server=91.99.138.108&port=155&secret=7hYDAQIAAQAH8AMDhuJMOt1tZWRpYS5zdGVhbXBvd2VyZWQuY29tbWVkaWEuc3RlYW1wb3dlcmVkLmNvbQ)__` |
| 26 | 46.62.141.92 | 155 | فعال | `tg://proxy?server=46.62.141.92&port=155&secret=ee07df7df7df7dffdffc07646f776e6c6f61642e77696e646f77737570646174652e636f6d` |
| 27 | 91.99.236.93 | 443 | فعال | `tg://proxy?server=91.99.236.93&port=443&secret=ee0000f00f0f775555fffffff5006e2e696d656469612e737465616d706f77657265642e636f6d` |
| 28 | 141.147.21.116 | 443 | فعال | `tg://proxy?server=141.147.21.116&port=443&secret=eed0d6e131bada5511fcce9584deadbeef6b65746161626f6e6c696e652e636f6d)[برای` |
| 29 | 91.99.105.128 | 8888 | فعال | `tg://proxy?server=91.99.105.128&port=8888&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 30 | 62.60.179.8 | 9880 | فعال | `tg://proxy?server=62.60.179.8&port=9880&secret=ee0000f00f0f775555fffffff5006e2e696d656469612e737465616d706f77657265642e636f6d****` |


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
