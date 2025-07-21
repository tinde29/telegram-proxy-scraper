# Telegram Proxy Scraper

[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Python](https://img.shields.io/badge/python-3.9-blue)](https://www.python.org/downloads/)
[![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/tinde29/telegram-proxy-scraper/issues)
[![Proxy Scraper Workflow](https://github.com/tinde29/telegram-proxy-scraper/actions/workflows/scraper.yml/badge.svg)](https://github.com/tinde29/telegram-proxy-scraper/actions/workflows/scraper.yml)
![GitHub last commit](https://img.shields.io/github/last-commit/tinde29/telegram-proxy-scraper)
![GitHub issues](https://img.shields.io/github/issues/tinde29/telegram-proxy-scraper)

**آخرین به‌روزرسانی پروکسی‌ها**: 21 July 2025, 18:58 UTC (به وقت ایران: 22:28)

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
| 1 | iran.needhost.ir | 443 | فعال | `tg://proxy?server=iran.needhost.ir&port=443&secret=7veb2r8DoV-UM_4TNesqGclpcmFuLm5lZWRob3N0Lmly` |
| 2 | 195.201.234.42 | 8888 | فعال | `tg://proxy?server=195.201.234.42&port=8888&secret=FgMBAgABAAH8AwOG4kw63Q` |
| 3 | cdn.opt-meli.info | 443 | فعال | `tg://proxy?server=cdn.opt-meli.info&port=443&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 4 | 109.104.154.230 | 443 | فعال | `tg://proxy?server=109.104.154.230&port=443&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t**` |
| 5 | 87.248.132.188 | 200 | فعال | `tg://proxy?server=87.248.132.188&port=200&secret=ee0000f00f0f775555fffffff5006e2e69646f776e6c6f61642e77696e646f77737570646174652e636f6d` |
| 6 | vip.bomberoo.co.uk | 155 | فعال | `tg://proxy?server=vip.bomberoo.co.uk&port=155&secret=7hYDAQIAAQAH8AMDhuJMOt1tZWRpYS5zdGVhbXBvd2VyZWQuY29tbWVkaWEuc3RlYW1wb3dlcmVkLmNvbQ)|` |
| 7 | silvermantain.cinere.info | 443 | فعال | `tg://proxy?server=silvermantain.cinere.info&port=443&secret=7hYDAQIAAQAB_AMDhuJMOt1tZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 8 | www.galacticfireworks.pro. | 888 | فعال | `tg://proxy?server=www.galacticfireworks.pro.&port=888&secret=ee0c30628212cbbd7ac519130205525d1569612e737465616d706f77657265642e636f6d)__` |
| 9 | irancell-hamrah.soren-mashin.ir. | 9741 | فعال | `tg://proxy?server=irancell-hamrah.soren-mashin.ir.&port=9741&secret=ee0000f00f0f775555fffffff5006e2e696d656469612e737465616d706f77657265642e636f6d)__` |
| 10 | 77.110.124.221 | 9741 | فعال | `tg://proxy?server=77.110.124.221&port=9741&secret=ee0000f00f0f775555fffffff5006e2e696d656469612e737465616d706f77657265642e636f6d****` |
| 11 | 91.99.178.38 | 888 | فعال | `tg://proxy?server=91.99.178.38&port=888&secret=7gwwYoISy716xRkTAgVSXRVpYS5zdGVhbXBvd2VyZWQuY29t` |
| 12 | 91.99.171.147 | 8888 | فعال | `tg://proxy?server=91.99.171.147&port=8888&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 13 | 5.255.97.157 | 443 | فعال | `tg://proxy?server=5.255.97.157&port=443&secret=15115115115115115115115115115115` |
| 14 | 91.134.57.71 | 443 | فعال | `tg://proxy?server=91.134.57.71&port=443&secret=ee915818963f39435ebc8d07feb36afcb76564782e636f6d` |
| 15 | 8.213.228.13 | 443 | فعال | `tg://proxy?server=8.213.228.13&port=443&secret=eef2cbc7ed088c732f9858b39443e181a3617a7572652e6d6963726f736f66742e636f6d` |
| 16 | upiran.irpower-f.ir | 443 | فعال | `tg://proxy?server=upiran.irpower-f.ir&port=443&secret=eed77db43ee3721f0fcb40a4ff63b5cd276D656469612E737465616D706F77657265642E636F6D` |
| 17 | 185.121.233.42 | 443 | فعال | `tg://proxy?server=185.121.233.42&port=443&secret=eed77db43ee3721f0fcb40a4ff63b5cd276D656469612E737465616D706F77657265642E636F6D` |
| 18 | 212.34.141.71 | 443 | فعال | `tg://proxy?server=212.34.141.71&port=443&secret=d77db43ee3721f0fcb40a4ff63b5cd27` |
| 19 | 46.62.149.198 | 8880 | فعال | `tg://proxy?server=46.62.149.198&port=8880&secret=7g__755555_W__vwv_ItLS0tLXd3dy5zZG8tLS0=` |
| 20 | 140.233.187.77 | 85 | فعال | `tg://proxy?server=140.233.187.77&port=85&secret=ee0000f00f0f775555fffffff5006e2e69646F776E6C6F61642E77696E646F77737570646174652E636F6D` |
| 21 | 62.60.177.174 | 8443 | فعال | `tg://proxy?server=62.60.177.174&port=8443&secret=FgMBAgABAAfwAwOG4kw63Q` |
| 22 | 157.180.93.115 | 443 | فعال | `tg://proxy?server=157.180.93.115&port=443&secret=ec742282124f04d318551341ead76457` |
| 23 | 62.60.177.195 | 9741 | فعال | `tg://proxy?server=62.60.177.195&port=9741&secret=ee0000f00f0f775555fffffff5006e2e696d656469612e737465616d706f77657265642e636f6d` |
| 24 | rak.hotelghooo.ir | 443 | فعال | `tg://proxy?server=rak.hotelghooo.ir&port=443&secret=ee000000000000000000000000000000007777772e4869646550726f78692e696f` |
| 25 | 5.255.126.224 | 443 | فعال | `tg://proxy?server=5.255.126.224&port=443&secret=ee1603010200010001fc030386e24c3add6d656469612e737465616d706f77657265642e636f6d` |
| 26 | 91.99.175.114 | 8888 | فعال | `tg://proxy?server=91.99.175.114&port=8888&secret=7gAA8A8Pd1VV` |
| 27 | 157.180.39.126 | 443 | فعال | `tg://proxy?server=157.180.39.126&port=443&secret=7HQighJPBNMYVRNB6tdkVw` |
| 28 | 87.248.132.85 | 44344 | فعال | `tg://proxy?server=87.248.132.85&port=44344&secret=ee0000f00f0f775555fffffff5006e2e696D656469612E737465616D706F77657265642E636F6D` |
| 29 | 45.152.164.19 | 70 | فعال | `tg://proxy?server=45.152.164.19&port=70&secret=7gffffffff_f_Adkb3dubG9hZC53aW5kb3dzdXBkYXRlLmNvbQ==` |
| 30 | 176.65.136.180 | 443 | فعال | `tg://proxy?server=176.65.136.180&port=443&secret=ee151151151151151151151151151151156d656469612e737465616d706f77657265642e636f6d` |


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
