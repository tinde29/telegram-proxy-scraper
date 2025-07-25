# Telegram Proxy Scraper

[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Python](https://img.shields.io/badge/python-3.9-blue)](https://www.python.org/downloads/)
[![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/tinde29/telegram-proxy-scraper/issues)
[![Proxy Scraper Workflow](https://github.com/tinde29/telegram-proxy-scraper/actions/workflows/scraper.yml/badge.svg)](https://github.com/tinde29/telegram-proxy-scraper/actions/workflows/scraper.yml)
![GitHub last commit](https://img.shields.io/github/last-commit/tinde29/telegram-proxy-scraper)
![GitHub issues](https://img.shields.io/github/issues/tinde29/telegram-proxy-scraper)

**آخرین به‌روزرسانی پروکسی‌ها**: 25 July 2025, 03:52 UTC (به وقت ایران: 07:22)

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
| 1 | 87.248.134.172 | 443 | فعال | `tg://proxy?server=87.248.134.172&port=443&secret=ee0000f00f0f775555fffffff5006e2e696D656469612E737465616D706F77657265642E636F6D` |
| 2 | 79.172.228.96 | 700 | فعال | `tg://proxy?server=79.172.228.96&port=700&secret=7gAA8A8Pd1VV9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t__` |
| 3 | 78.46.240.236 | 443 | فعال | `tg://proxy?server=78.46.240.236&port=443&secret=0c30628212cbbd7ac519130205525d15` |
| 4 | 103.215.221.15 | 8880 | فعال | `tg://proxy?server=103.215.221.15&port=8880&secret=ee6b8f9952c8f9c4e043cc3f24d0ae1bf47a756c612e6972` |
| 5 | 140.233.187.83 | 70 | فعال | `tg://proxy?server=140.233.187.83&port=70&secret=7td9tD7jch8Py0Ck_2O1zSdtZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 6 | 88.198.109.90 | 6968 | فعال | `tg://proxy?server=88.198.109.90&port=6968&secret=adf40f46d165230637065edeeac211a9` |
| 7 | 78.47.224.218 | 155 | فعال | `tg://proxy?server=78.47.224.218&port=155&secret=7gffffffff_f_Adkb3dubG9hZC53aW5kb3dzdXBkYXRlLmNvbQ` |
| 8 | 45.13.226.180 | 8882 | فعال | `tg://proxy?server=45.13.226.180&port=8882&secret=eed700433aba3557d5e83d82beb4ab735873332e616d617a6f6e6177732e636f6d` |
| 9 | 157.180.125.85 | 98 | فعال | `tg://proxy?server=157.180.125.85&port=98&secret=1320PuNyHw_LQKT_Y7XNJw==` |
| 10 | mtproxy10.alphacyber.org | 443 | فعال | `tg://proxy?server=mtproxy10.alphacyber.org&port=443&secret=dde5ceff7c8a4a80fcad3dae7d23f3ac65` |
| 11 | 79.172.228.57 | 70 | فعال | `tg://proxy?server=79.172.228.57&port=70&secret=ee0000f00f0f775555fffffff5006e2e696D656469612E737465616D706F77657265642E636F6D` |
| 12 | 163.123.141.136 | 443 | فعال | `tg://proxy?server=163.123.141.136&port=443&secret=ddf900af441604263a084c1aa73af331ac` |
| 13 | 185.253.1.22 | 333 | فعال | `tg://proxy?server=185.253.1.22&port=333&secret=7rXpXsHm4qJ_nKJvoq_oq_ptZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 14 | 93.88.205.35 | 85 | فعال | `tg://proxy?server=93.88.205.35&port=85&secret=7gAA8A8Pd1VV__9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 15 | 47.236.248.226 | 443 | فعال | `tg://proxy?server=47.236.248.226&port=443&secret=ee0857670d0264d45aa725034b90631f5d617a7572652e6d6963726f736f66742e636f6d` |
| 16 | 95.216.201.145 | 9091 | فعال | `tg://proxy?server=95.216.201.145&port=9091&secret=7ggggggg-r-r-r__AAAAAAAtLmNvbS0=)__` |
| 17 | 89.251.10.33 | 6443 | فعال | `tg://proxy?server=89.251.10.33&port=6443&secret=ee151151151151151151151151151151156d656469612e737465616d706f77657265642e636f6d)**` |
| 18 | 116.203.81.58 | 8888 | فعال | `tg://proxy?server=116.203.81.58&port=8888&secret=FgMBAgABAAH8AwOG4kw63Q` |
| 19 | 500.meli.zban-mas.info | 8888 | فعال | `tg://proxy?server=500.meli.zban-mas.info&port=8888&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 20 | SIGNAL.irpower-b.ir | 443 | فعال | `tg://proxy?server=SIGNAL.irpower-b.ir&port=443&secret=eed77db43ee3721f0fcb40a4ff63b5cd276D656469612E737465616D706F77657265642E636F6D` |
| 21 | 151.244.50.48 | 443 | فعال | `tg://proxy?server=151.244.50.48&port=443&secret=eed77db43ee3721f0fcb40a4ff63b5cd276D656469612E737465616D706F77657265642E636F6D` |
| 22 | 62.60.176.253 | 443 | فعال | `tg://proxy?server=62.60.176.253&port=443&secret=eed77db43ee3721f0fcb40a4ff63b5cd276D656469612E737465616D706F77657265642E636F6D` |
| 23 | 3.dfff.cloudflare.com.nokia.com.co.uk.do_yo.want_to.clash_with.this.www.microsoft.com.there_is_no.place_like.localhost.www.bing.com.count_with_me.cyou.net.digikala.com.www.enamad.ir.www.google.com.again_to_fight.everyone.i_am.the_internet.zban-df.info | 8888 | فعال | `tg://proxy?server=3.dfff.cloudflare.com.nokia.com.co.uk.do_yo.want_to.clash_with.this.www.microsoft.com.there_is_no.place_like.localhost.www.bing.com.count_with_me.cyou.net.digikala.com.www.enamad.ir.www.google.com.again_to_fight.everyone.i_am.the_internet.zban-df.info&port=8888&secret=FgMBAgABAAH8AwOG4kw63Q` |
| 24 | 31.184.172.121 | 2086 | فعال | `tg://proxy?server=31.184.172.121&port=2086&secret=1f9fdd1eddffba2661772fa299eef89c` |
| 25 | 185.117.0.199 | 8882 | فعال | `tg://proxy?server=185.117.0.199&port=8882&secret=eed700433aba3557d5e83d82beb4ab735873332e616d617a6f6e6177732e636f6d` |
| 26 | 144.76.220.86 | 443 | فعال | `tg://proxy?server=144.76.220.86&port=443&secret=7s8J5YYVhvOdr-WqHy_58gVtZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 27 | 88.198.108.29 | 443 | فعال | `tg://proxy?server=88.198.108.29&port=443&secret=DDBighLLvXrFGRMCBVJdFQ` |
| 28 | 95.216.22.207 | 443 | فعال | `tg://proxy?server=95.216.22.207&port=443&secret=7HQighJPBNMYVRNB6tdkVw` |
| 29 | 4.dfff.cloudflare.com.nokia.com.co.uk.do_yo.want_to.clash_with.this.www.microsoft.com.there_is_no.place_like.localhost.www.bing.com.count_with_me.cyou.net.digikala.com.www.enamad.ir.www.google.com.again_to_fight.everyone.i_am.the_internet.zban-df.info | 8888 | فعال | `tg://proxy?server=4.dfff.cloudflare.com.nokia.com.co.uk.do_yo.want_to.clash_with.this.www.microsoft.com.there_is_no.place_like.localhost.www.bing.com.count_with_me.cyou.net.digikala.com.www.enamad.ir.www.google.com.again_to_fight.everyone.i_am.the_internet.zban-df.info&port=8888&secret=FgMBAgABAAH8AwOG4kw63Q` |
| 30 | ommmm.aychichi.ir | 443 | فعال | `tg://proxy?server=ommmm.aychichi.ir&port=443&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t)__` |


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
