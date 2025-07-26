# Telegram Proxy Scraper

[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Python](https://img.shields.io/badge/python-3.9-blue)](https://www.python.org/downloads/)
[![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/tinde29/telegram-proxy-scraper/issues)
[![Proxy Scraper Workflow](https://github.com/tinde29/telegram-proxy-scraper/actions/workflows/scraper.yml/badge.svg)](https://github.com/tinde29/telegram-proxy-scraper/actions/workflows/scraper.yml)
![GitHub last commit](https://img.shields.io/github/last-commit/tinde29/telegram-proxy-scraper)
![GitHub issues](https://img.shields.io/github/issues/tinde29/telegram-proxy-scraper)

**آخرین به‌روزرسانی پروکسی‌ها**: 26 July 2025, 03:49 UTC (به وقت ایران: 07:19)

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
| 1 | 157.180.34.27 | 63844 | فعال | `tg://proxy?server=157.180.34.27&port=63844&secret=7qG2Zs5925jkwylckXCRkhNfLXMwLmJlby4taXI=)__` |
| 2 | 195.201.53.21 | 404 | فعال | `tg://proxy?server=195.201.53.21&port=404&secret=eeNEgYdJvXrFGRMCIMJdCQ==` |
| 3 | 57.129.92.216 | 70 | فعال | `tg://proxy?server=57.129.92.216&port=70&secret=eeb7faf1ae6383bae0bdc3c4289759ce426d656469612e737465616d706f77657265642e636f6d` |
| 4 | 19.Ir.ir.ir.ir.ir.zban-mas.info | 8888 | فعال | `tg://proxy?server=19.Ir.ir.ir.ir.ir.zban-mas.info&port=8888&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t)__` |
| 5 | 94.130.54.26 | 3443 | فعال | `tg://proxy?server=94.130.54.26&port=3443&secret=0c30628212cbbd7ac519130205525d15` |
| 6 | 83.147.255.85 | 443 | فعال | `tg://proxy?server=83.147.255.85&port=443&secret=EE1603010200010007f0030386e24c3add646f776e6c6f61642e77696e646f77737570646174652e636f6` |
| 7 | 140.233.187.91 | 8080 | فعال | `tg://proxy?server=140.233.187.91&port=8080&secret=eed77db43ee3721f0fcb40a4ff63b5cd276d656469612e737465616d706f77657265642e636f6d)/[ایرانسل](https://t.me/proxy?server=140.233.187.63` |
| 8 | 4.meli.zban-mas.info | 8888 | فعال | `tg://proxy?server=4.meli.zban-mas.info&port=8888&secret=7gAA8A8Pd1VV////9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 9 | 91.134.57.71 | 443 | فعال | `tg://proxy?server=91.134.57.71&port=443&secret=ee915818963f39435ebc8d07feb36afcb76564782e636f6d` |
| 10 | 62.60.178.33 | 443 | فعال | `tg://proxy?server=62.60.178.33&port=443&secret=7hYDAQIAAQAH8AMDhuJMOt1tZWRpYS5zdGVhbXBvd2VyZWQuY29tbWVkaWEuc3RlYW1wb3dlcmVkLmNvbQ)`` |
| 11 | 157.180.90.85 | 443 | فعال | `tg://proxy?server=157.180.90.85&port=443&secret=1603010200010001fc030386e24c3add` |
| 12 | 6.meli.meli.zban-mas.info | 8888 | فعال | `tg://proxy?server=6.meli.meli.zban-mas.info&port=8888&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t)__` |
| 13 | 62.60.176.59 | 443 | فعال | `tg://proxy?server=62.60.176.59&port=443&secret=7hYDAQIAAQAH8AMDhuJMOt1tZWRpYS5zdGVhbXBvd2VyZWQuY29tbWVkaWEuc3RlYW1wb3dlcmVkLmNvbQ)|` |
| 14 | bmw.hezarsh-mashal0.co.vjhkgttrrhks-sdcj.co.uk.pwkxjjrhks-skci.co.uk.pwkxjjrhks-ikcj.co.uk.fskxjjrhks-rkcr.co.uk.mstukxjjrhkss-jscj.co.uk. | 7443 | فعال | `tg://proxy?server=bmw.hezarsh-mashal0.co.vjhkgttrrhks-sdcj.co.uk.pwkxjjrhks-skci.co.uk.pwkxjjrhks-ikcj.co.uk.fskxjjrhks-rkcr.co.uk.mstukxjjrhkss-jscj.co.uk.&port=7443&secret=eeRighJJvXrFGRMCIMJdCQ)**` |
| 15 | 91.99.195.241 | 69 | فعال | `tg://proxy?server=91.99.195.241&port=69&secret=7pVZ3VtL_Wuy49KeR-ZTRlB3d3cuc3BlZWR0ZXN0Lm5ldA==` |
| 16 | arvan.irpower-g.ir | 443 | فعال | `tg://proxy?server=arvan.irpower-g.ir&port=443&secret=ee07df7df7df7dfffffdfffffffffffc07646f776e6c6f61642e77696e646f77737570646174652e636f6d‌|‌[پروکسی](https://t.me/proxy?server=NoVA.irpower-g.ir` |
| 17 | 2.dfff.cloudflare.com.nokia.com.co.uk.do_yo.want_to.clash_with.this.www.microsoft.com.there_is_no.place_like.localhost.www.bing.com.count_with_me.cyou.net.digikala.com.www.enamad.ir.www.google.com.again_to_fight.everyone.i_am.the_internet.zban-df.info | 8888 | فعال | `tg://proxy?server=2.dfff.cloudflare.com.nokia.com.co.uk.do_yo.want_to.clash_with.this.www.microsoft.com.there_is_no.place_like.localhost.www.bing.com.count_with_me.cyou.net.digikala.com.www.enamad.ir.www.google.com.again_to_fight.everyone.i_am.the_internet.zban-df.info&port=8888&secret=FgMBAgABAAH8AwOG4kw63Q` |
| 18 | 195.200.31.115 | 443 | فعال | `tg://proxy?server=195.200.31.115&port=443&secret=7rXpXsHm4qJ_nKJvoq_oq_ptZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 19 | 49.12.38.200 | 155 | فعال | `tg://proxy?server=49.12.38.200&port=155&secret=dd1603010200010001fc030386e24c3add` |
| 20 | 91.99.199.235 | 443 | فعال | `tg://proxy?server=91.99.199.235&port=443&secret=eec862057ba49a7ecdf0ad4eb44cd5bb11646f776e6c6f61642e77696e646f77737570646174652e636f6d` |
| 21 | 46.62.144.121 | 70 | فعال | `tg://proxy?server=46.62.144.121&port=70&secret=7gAA8A8Pd1VV____9QBuLmktLXd-Z28tLS0=` |
| 22 | lock.irpower-b.ir | 443 | فعال | `tg://proxy?server=lock.irpower-b.ir&port=443&secret=eed77db43ee3721f0fcb40a4ff63b5cd276D656469612E737465616D706F77657265642E636F6D` |
| 23 | 87.248.132.44 | 200 | فعال | `tg://proxy?server=87.248.132.44&port=200&secret=eeNEgYdJvXrFGRMCIMJdCQ)**` |
| 24 | 185.142.95.21 | 2028 | فعال | `tg://proxy?server=185.142.95.21&port=2028&secret=dd2028b5afa0e6d701acec3cd9bb8a902b` |
| 25 | 87.248.132.85 | 44344 | فعال | `tg://proxy?server=87.248.132.85&port=44344&secret=ee0000f00f0f775555fffffff5006e2e696D656469612E737465616D706F77657265642E636F6D` |
| 26 | 167.235.169.138 | 443 | فعال | `tg://proxy?server=167.235.169.138&port=443&secret=7gffffffff_f_Adkb3dubG9hZC53aW5kb3dzdXBkYXRlLmNvbQ` |
| 27 | 77.246.110.193 | 443 | فعال | `tg://proxy?server=77.246.110.193&port=443&secret=eeNEgYdJvXrFGRMCIMJdCQRueWVrdGFuZXQuY29tZmFyYWthdi5jb212YW4ubmFqdmEuY29tAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA)**` |
| 28 | 62.60.178.146 | 443 | فعال | `tg://proxy?server=62.60.178.146&port=443&secret=7hYDAQIAAQAH8AMDhuJMOt1tZWRpYS5zdGVhbXBvd2VyZWQuY29tbWVkaWEuc3RlYW1wb3dlcmVkLmNvbQ` |
| 29 | 91.107.172.155 | 443 | فعال | `tg://proxy?server=91.107.172.155&port=443&secret=eeNEgYdJvXrFGRMCIMJdCQ` |
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
