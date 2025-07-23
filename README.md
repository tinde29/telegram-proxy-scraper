# Telegram Proxy Scraper

[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Python](https://img.shields.io/badge/python-3.9-blue)](https://www.python.org/downloads/)
[![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/tinde29/telegram-proxy-scraper/issues)
[![Proxy Scraper Workflow](https://github.com/tinde29/telegram-proxy-scraper/actions/workflows/scraper.yml/badge.svg)](https://github.com/tinde29/telegram-proxy-scraper/actions/workflows/scraper.yml)
![GitHub last commit](https://img.shields.io/github/last-commit/tinde29/telegram-proxy-scraper)
![GitHub issues](https://img.shields.io/github/issues/tinde29/telegram-proxy-scraper)

**آخرین به‌روزرسانی پروکسی‌ها**: 23 July 2025, 03:54 UTC (به وقت ایران: 07:24)

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
| 1 | 91.99.165.90 | 443 | فعال | `tg://proxy?server=91.99.165.90&port=443&secret=7gAA8A8Pd1VV____9QBuLmktLXcuZ28tLS0` |
| 2 | iran.needhost.ir | 443 | فعال | `tg://proxy?server=iran.needhost.ir&port=443&secret=7veb2r8DoV-UM_4TNesqGclpcmFuLm5lZWRob3N0Lmly` |
| 3 | 85.198.111.90 | 443 | فعال | `tg://proxy?server=85.198.111.90&port=443&secret=7td9tD7jch8Py0Ck_2O1zSdtZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 4 | 89.251.10.4 | 6443 | فعال | `tg://proxy?server=89.251.10.4&port=6443&secret=ee151151151151151151151151151151156d656469612e737465616d706f77657265642e636f6d)__` |
| 5 | 87.248.134.203 | 443 | فعال | `tg://proxy?server=87.248.134.203&port=443&secret=ee0000f00f0f775555fffffff5006e2e696D656469612E737465616D706F77657265642E636F6D)__` |
| 6 | 87.248.132.36 | 70 | فعال | `tg://proxy?server=87.248.132.36&port=70&secret=eed77db43ee3721f0fcb40a4ff63b5cd276D656469612E737465616D706F77657265642E636F6D)[**` |
| 7 | 151.244.85.32 | 70 | فعال | `tg://proxy?server=151.244.85.32&port=70&secret=eed77db43ee3721f0fcb40a4ff63b5cd276D656469612E737465616D706F77657265642E636F6` |
| 8 | 47.242.197.105 | 443 | فعال | `tg://proxy?server=47.242.197.105&port=443&secret=ee3405ffc0579d0ef9c0438f288bc8087a617a7572652e6d6963726f736f66742e636f6d` |
| 9 | 146.103.105.74 | 443 | فعال | `tg://proxy?server=146.103.105.74&port=443&secret=7gAA8A8Pd1VV____9QBuLmktLS1-wrHinJMtLS0` |
| 10 | 65.108.80.13 | 443 | فعال | `tg://proxy?server=65.108.80.13&port=443&secret=3QAAAAAAAAAAAAAAAAAAAAA=` |
| 11 | bahbah.khoreshtsabzi.ir | 8585 | فعال | `tg://proxy?server=bahbah.khoreshtsabzi.ir&port=8585&secret=dd5d5b15b207cd8974a5ae0585282bc510` |
| 12 | 9891.Ir.ir.ir.ir.ir.zban-mas.info | 8888 | فعال | `tg://proxy?server=9891.Ir.ir.ir.ir.ir.zban-mas.info&port=8888&secret=7gAA8A8Pd1VV9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t__` |
| 13 | 87.248.132.39 | 85 | فعال | `tg://proxy?server=87.248.132.39&port=85&secret=ee0000f00f0f775555fffffff5006e2e69646F776E6C6F61642E77696E646F77737570646174652E636F6D` |
| 14 | ae.mohs1736.sbs | 4637 | فعال | `tg://proxy?server=ae.mohs1736.sbs&port=4637&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t)__` |
| 15 | 157.180.93.68 | 888 | فعال | `tg://proxy?server=157.180.93.68&port=888&secret=79e344818749bd7ac519130220c25d09` |
| 16 | 46.249.35.164 | 85 | فعال | `tg://proxy?server=46.249.35.164&port=85&secret=ee0000f00f0f775555fffffff5006e2e69646F776E6C6F61642E77696E646F77737570646174652E636F6D` |
| 17 | 213.145.71.35 | 443 | فعال | `tg://proxy?server=213.145.71.35&port=443&secret=eed77db43ee3721f0fcb40a4ff63b5cd276D656469612E737465616D706F77657265642E636F6D` |
| 18 | 87.248.134.77 | 200 | فعال | `tg://proxy?server=87.248.134.77&port=200&secret=eeNEgYdJvXrFGRMCIMJdCQ` |
| 19 | 94.130.70.120 | 200 | فعال | `tg://proxy?server=94.130.70.120&port=200&secret=eeNEgYdJvXrFGRMCIMJdCQ` |
| 20 | 91.99.201.44 | 443 | فعال | `tg://proxy?server=91.99.201.44&port=443&secret=eec862057ba49a7ecdf0ad4eb44cd5bb11646f776e6c6f61642e77696e646f77737570646174652e636f6d)__` |
| 21 | soos-turk.nuremborg-hamborg.dodos-codam.jojo19.ir | 443 | فعال | `tg://proxy?server=soos-turk.nuremborg-hamborg.dodos-codam.jojo19.ir&port=443&secret=7gD_AA___wD_9VVf______VtZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 22 | 203.25.108.13 | 85 | فعال | `tg://proxy?server=203.25.108.13&port=85&secret=ee0000f00f0f775555fffffff5006e2e69646F776E6C6F61642E77696E646F77737570646174652E636F6D` |
| 23 | Dashakol.77.44-207-58.ir | 70 | فعال | `tg://proxy?server=Dashakol.77.44-207-58.ir&port=70&secret=7gAA8A8Pd1VV____9QBuLmktLXd-Z28tLS0=` |
| 24 | 5.255.126.122 | 443 | فعال | `tg://proxy?server=5.255.126.122&port=443&secret=7hYDAQIAAQAB_AMDhuJMOt1tZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 25 | 8.220.185.235 | 443 | فعال | `tg://proxy?server=8.220.185.235&port=443&secret=eee8725affe357534b2ff1e6a1727b47ee617a7572652e6d6963726f736f66742e636f6d` |
| 26 | 488.ir.ir.ir.ir.ir.zban-mas.info | 8888 | فعال | `tg://proxy?server=488.ir.ir.ir.ir.ir.zban-mas.info&port=8888&secret=7gAA8A8Pd1VV__9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 27 | 157.180.95.196 | 888 | فعال | `tg://proxy?server=157.180.95.196&port=888&secret=79e344818749bd7ac519130220c25d09` |
| 28 | 4.meli.zban-mas.info | 8888 | فعال | `tg://proxy?server=4.meli.zban-mas.info&port=8888&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 29 | 157.180.126.9 | 8888 | فعال | `tg://proxy?server=157.180.126.9&port=8888&secret=FgMBAgABAAH8AwOG4kw63Q` |
| 30 | tcp.ircheck-j.ir | 70 | فعال | `tg://proxy?server=tcp.ircheck-j.ir&port=70&secret=eed77db43ee3721f0fcb40a4ff63b5cd276D656469612E737465616D706F77657265642E636F6D)__` |


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
