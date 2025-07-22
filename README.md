# Telegram Proxy Scraper

[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Python](https://img.shields.io/badge/python-3.9-blue)](https://www.python.org/downloads/)
[![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/tinde29/telegram-proxy-scraper/issues)
[![Proxy Scraper Workflow](https://github.com/tinde29/telegram-proxy-scraper/actions/workflows/scraper.yml/badge.svg)](https://github.com/tinde29/telegram-proxy-scraper/actions/workflows/scraper.yml)
![GitHub last commit](https://img.shields.io/github/last-commit/tinde29/telegram-proxy-scraper)
![GitHub issues](https://img.shields.io/github/issues/tinde29/telegram-proxy-scraper)

**آخرین به‌روزرسانی پروکسی‌ها**: 22 July 2025, 18:58 UTC (به وقت ایران: 22:28)

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
| 1 | kheybar.co.uk | 443 | فعال | `tg://proxy?server=kheybar.co.uk&port=443&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 2 | 62.60.176.254 | 443 | فعال | `tg://proxy?server=62.60.176.254&port=443&secret=eed77db43ee3721f0fcb40a4ff63b5cd276D656469612E737465616D706F77657265642E636F6D` |
| 3 | 87.229.100.237 | 443 | فعال | `tg://proxy?server=87.229.100.237&port=443&secret=eeRighJJvXrFGRMCIMJdCQ` |
| 4 | 151.244.85.20 | 70 | فعال | `tg://proxy?server=151.244.85.20&port=70&secret=ee07df7df7df7dfffffdfffffffffffc07646f776e6c6f61642e77696e646f77737570646174652e636f6d` |
| 5 | 23.88.96.144 | 155 | فعال | `tg://proxy?server=23.88.96.144&port=155&secret=7HQighJPBNMYVRNB6tdkVw` |
| 6 | 87.248.134.172 | 443 | فعال | `tg://proxy?server=87.248.134.172&port=443&secret=ee0000f00f0f775555fffffff5006e2e696D656469612E737465616D706F77657265642E636F6D)__` |
| 7 | Sariee.45.712.38-82.ir | 443 | فعال | `tg://proxy?server=Sariee.45.712.38-82.ir&port=443&secret=7hBKyBmZ41cUX4K5nIpow3ltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 8 | 94.130.218.244 | 443 | فعال | `tg://proxy?server=94.130.218.244&port=443&secret=EERighJJvXrFGRMCIMJdCQ` |
| 9 | 193.109.120.106 | 443 | فعال | `tg://proxy?server=193.109.120.106&port=443&secret=EE100404ff0f48064fffffff9001b8696d696d656469612e737465616d706f77657265642e636f6d` |
| 10 | 77.238.253.117 | 443 | فعال | `tg://proxy?server=77.238.253.117&port=443&secret=7gffffffff_f_Adkb3dubG9hZC53aW5kb3dzdXBkYXRlLmNvbQ` |
| 11 | 91.99.161.12 | 70 | فعال | `tg://proxy?server=91.99.161.12&port=70&secret=7gAA8A8Pd1VV____9QBuLmktLXcuZ28tLS0=` |
| 12 | 138.201.51.101 | 8443 | فعال | `tg://proxy?server=138.201.51.101&port=8443&secret=DDBighLLvXrFGRMCBVJdFQ==` |
| 13 | sebro.sheshko.info | 443 | فعال | `tg://proxy?server=sebro.sheshko.info&port=443&secret=ee1603010200010001fc030386e24c3add6d656469612e737465616d706f77657265642e636f6d` |
| 14 | 79.172.228.73 | 85 | فعال | `tg://proxy?server=79.172.228.73&port=85&secret=ee0000f00f0f775555fffffff5006e2e69646F776E6C6F61642E77696E646F77737570646174652E636F6D` |
| 15 | 89.251.10.22 | 443 | فعال | `tg://proxy?server=89.251.10.22&port=443&secret=ee151151151151151151151151151151156d656469612e737465616d706f77657265642e636f6d` |
| 16 | 91.99.202.250 | 888 | فعال | `tg://proxy?server=91.99.202.250&port=888&secret=ee0c30628212cbbd7ac519130205525d1569612e737465616d706f77657265642e636f6d` |
| 17 | 8.213.228.13 | 443 | فعال | `tg://proxy?server=8.213.228.13&port=443&secret=7vLLx` |
| 18 | 178.130.41.215 | 443 | فعال | `tg://proxy?server=178.130.41.215&port=443&secret=7rXpXsHm4qJ_nKJvoq_oq_ptZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 19 | response.cinere.info | 443 | فعال | `tg://proxy?server=response.cinere.info&port=443&secret=7hYDAQIAAQAB_AMDhuJMOt1tZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 20 | www.newtcpconnectiodo.store | 888 | فعال | `tg://proxy?server=www.newtcpconnectiodo.store&port=888&secret=ee0c30628212cbbd7ac519130205525d1569612e737465616d706f77657265642e636f6d` |
| 21 | 176.65.128.50 | 155 | فعال | `tg://proxy?server=176.65.128.50&port=155&secret=ee07df7df7df7dffdffc07646f776e6c6f61642e77696e646f77737570646174652e636f6d|[پروکسی](tg://proxy?server=176.65.128.51` |
| 22 | 1.df.cloudflare.com.nokia.com.co.uk.do_yo.want_to.clash_with.this.www.microsoft.com.there_is_no.place_like.localhost.www.bing.com.count_with_me.cyou.net.digikala.com.www.enamad.ir.www.google.com.again_to_fight.everyone.i_am.the_internet.brobalair.store | 8888 | فعال | `tg://proxy?server=1.df.cloudflare.com.nokia.com.co.uk.do_yo.want_to.clash_with.this.www.microsoft.com.there_is_no.place_like.localhost.www.bing.com.count_with_me.cyou.net.digikala.com.www.enamad.ir.www.google.com.again_to_fight.everyone.i_am.the_internet.brobalair.store&port=8888&secret=FgMBAgABAAH8AwOG4kw63Q` |
| 23 | 176.124.32.175 | 443 | فعال | `tg://proxy?server=176.124.32.175&port=443&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 24 | 5.255.114.52 | 443 | فعال | `tg://proxy?server=5.255.114.52&port=443&secret=15115115115115115115115115115115` |
| 25 | 163.123.141.136 | 443 | فعال | `tg://proxy?server=163.123.141.136&port=443&secret=7vkAr0QWBCY6CEwapzrzMaxnb29nbGUuY29t` |
| 26 | 87.248.132.67 | 200 | فعال | `tg://proxy?server=87.248.132.67&port=200&secret=eeNEgYdJvXrFGRMCIMJdCQ` |
| 27 | 4.e7777.cloudflare.com.nokia.com.co.uk.do_yo.want_to.clash_with.this.www.microsoft.com.there_is_no.place_like.localhost.www.bing.com.count_with_me.cyou.net.digikala.com.www.enamad.ir.www.google.com.again_to_fight.everyone.i_am.zban-mas.info | 8888 | فعال | `tg://proxy?server=4.e7777.cloudflare.com.nokia.com.co.uk.do_yo.want_to.clash_with.this.www.microsoft.com.there_is_no.place_like.localhost.www.bing.com.count_with_me.cyou.net.digikala.com.www.enamad.ir.www.google.com.again_to_fight.everyone.i_am.zban-mas.info&port=8888&secret=FgMBAgABAAH8AwOG4kw63Q` |
| 28 | 81.12.96.203 | 1000 | فعال | `tg://proxy?server=81.12.96.203&port=1000&secret=ee4714faa05f25f39c7f1ddc4438110bd77777772e63626c6f756463646e2e636f6d` |
| 29 | new-pio-iran-ck-uk-ir.zx2hgujoiah-xy1xutr021-2tk.info | 8443 | فعال | `tg://proxy?server=new-pio-iran-ck-uk-ir.zx2hgujoiah-xy1xutr021-2tk.info&port=8443&secret=7gAA8A8Pd1VV____9QBuLmktLXcuZ28tLS0=)__` |
| 30 | 87.248.132.17 | 343 | فعال | `tg://proxy?server=87.248.132.17&port=343&secret=eed77db43ee3721f0fcb40a4ff63b5cd276D656469612E737465616D706F77657265642E636F6D` |


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
