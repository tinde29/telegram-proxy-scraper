# Telegram Proxy Scraper

[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Python](https://img.shields.io/badge/python-3.9-blue)](https://www.python.org/downloads/)
[![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/tinde29/telegram-proxy-scraper/issues)
[![Proxy Scraper Workflow](https://github.com/tinde29/telegram-proxy-scraper/actions/workflows/scraper.yml/badge.svg)](https://github.com/tinde29/telegram-proxy-scraper/actions/workflows/scraper.yml)
![GitHub last commit](https://img.shields.io/github/last-commit/tinde29/telegram-proxy-scraper)
![GitHub issues](https://img.shields.io/github/issues/tinde29/telegram-proxy-scraper)

**آخرین به‌روزرسانی پروکسی‌ها**: 25 July 2025, 18:57 UTC (به وقت ایران: 22:27)

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
| 1 | vip.abanol1.info | 70 | فعال | `tg://proxy?server=vip.abanol1.info&port=70&secret=eed77db43ee3721f0fcb40a4ff63b5cd276d656469612e737465616d706f77657265642e636f6d)`` |
| 2 | 195.200.19.233 | 443 | فعال | `tg://proxy?server=195.200.19.233&port=443&secret=1320PuNyHw_LQKT_Y7XNJw` |
| 3 | 151.244.50.72 | 200 | فعال | `tg://proxy?server=151.244.50.72&port=200&secret=eeNEgYdJvXrFGRMCIMJdCQ` |
| 4 | 94.130.48.73 | 8443 | فعال | `tg://proxy?server=94.130.48.73&port=8443&secret=DDBighLLvhhgexxguuuuuuXrFGRMCBVJdFQ==` |
| 5 | 91.99.100.55 | 70 | فعال | `tg://proxy?server=91.99.100.55&port=70&secret=eed77db43ee3721f0fcb40a4ff63b5cd276d656469612e737465616d706f77657265642e636f6d` |
| 6 | 8483.Ir.ir.ir.ir.ir.zban-mas.info | 8888 | فعال | `tg://proxy?server=8483.Ir.ir.ir.ir.ir.zban-mas.info&port=8888&secret=7gAA8A8Pd1VV9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 7 | 138.201.196.220 | 8443 | فعال | `tg://proxy?server=138.201.196.220&port=8443&secret=DDBighLLvXrFGRMCBVJdFQ==` |
| 8 | 185.253.1.22 | 333 | فعال | `tg://proxy?server=185.253.1.22&port=333&secret=7rXpXsHm4qJ_nKJvoq_oq_ptZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 9 | 151.244.44.3 | 85 | فعال | `tg://proxy?server=151.244.44.3&port=85&secret=ee0000f00f0f775555fffffff5006e2e696d656469612e737465616d706f77657265642e636f6d` |
| 10 | 109.104.154.207 | 443 | فعال | `tg://proxy?server=109.104.154.207&port=443&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 11 | 57.129.95.177 | 443 | فعال | `tg://proxy?server=57.129.95.177&port=443&secret=ee235259a42975595e29ded06bd1371d497777772e7363616c657161792e636f6d` |
| 12 | 94.130.54.26 | 7149 | فعال | `tg://proxy?server=94.130.54.26&port=7149&secret=DDBighLLvXrFGRMCBVJdFQ==` |
| 13 | Optal.62.37-68-174.ir | 443 | فعال | `tg://proxy?server=Optal.62.37-68-174.ir&port=443&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 14 | moon.ddbighll.ir | 443 | فعال | `tg://proxy?server=moon.ddbighll.ir&port=443&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 15 | 50.7.85.218 | 443 | فعال | `tg://proxy?server=50.7.85.218&port=443&secret=eee7ce9f4679bfc87bb93390ed56e2c9686170742d6d6972726f722e6f7267` |
| 16 | 116.202.83.134 | 404 | فعال | `tg://proxy?server=116.202.83.134&port=404&secret=eeNEgYdJvXrFGRMCIMJdCQ` |
| 17 | 46.62.138.143 | 51886 | فعال | `tg://proxy?server=46.62.138.143&port=51886&secret=eeee52c867dc75983faf4bb37f91d5164f6d656469612e737465616d706f77657265642e636f6d` |
| 18 | 488.Ir.ir.ir.ir.ir.zban-mas.info | 8888 | فعال | `tg://proxy?server=488.Ir.ir.ir.ir.ir.zban-mas.info&port=8888&secret=7gAA8A8Pd1VV__9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 19 | 95.217.77.168 | 443 | فعال | `tg://proxy?server=95.217.77.168&port=443&secret=iORid5lJ237IiBMGYMQMdw==` |
| 20 | halftime.parsintalk.ir | 443 | فعال | `tg://proxy?server=halftime.parsintalk.ir&port=443&secret=7hYDAQIAAQAB_AMDhuJMOt1tZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 21 | siteimprove.ir | 443 | فعال | `tg://proxy?server=siteimprove.ir&port=443&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 22 | 164.90.237.85 | 80 | فعال | `tg://proxy?server=164.90.237.85&port=80&secret=3V9HEDbXrf_pCKa76RM2stc` |
| 23 | 91.99.171.147 | 8888 | فعال | `tg://proxy?server=91.99.171.147&port=8888&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29` |
| 24 | 185.117.0.135 | 8882 | فعال | `tg://proxy?server=185.117.0.135&port=8882&secret=eed700433aba3557d5e83d82beb4ab735873332e616d617a6f6e6177732e636f6d` |
| 25 | 77.238.233.217 | 443 | فعال | `tg://proxy?server=77.238.233.217&port=443&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29tفیلترشکن` |
| 26 | 140.233.187.210 | 443 | فعال | `tg://proxy?server=140.233.187.210&port=443&secret=eed77db43ee3721f0fcb40a4ff63b5cd276d656469612e737465616d706f77657265642e636f6d` |
| 27 | 62.60.179.150 | 343 | فعال | `tg://proxy?server=62.60.179.150&port=343&secret=eed77db43ee3721f0fcb40a4ff63b5cd276d656469612e737465616d706f77657265642e636f6d` |
| 28 | 87.248.132.36 | 70 | فعال | `tg://proxy?server=87.248.132.36&port=70&secret=eed77db43ee3721f0fcb40a4ff63b5cd276D656469612E737465616D706F77657265642E636F6D)[**` |
| 29 | 91.201.115.4 | 443 | فعال | `tg://proxy?server=91.201.115.4&port=443&secret=eeNEgYdJvXrFGRMCIMJdCQRueWVrdGFuZXQuY29tZmFyYWthdi5jb212YW4ubmFqdmEuY29tAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAhttps://t.me/proxy?server=91.201.115.4` |
| 30 | 193.3.190.75 | 85 | فعال | `tg://proxy?server=193.3.190.75&port=85&secret=ee0c30628212cbbd7ac519130205525d1569612e737465616d706f77657265642e636f6d` |


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
