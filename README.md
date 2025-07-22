# Telegram Proxy Scraper

[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Python](https://img.shields.io/badge/python-3.9-blue)](https://www.python.org/downloads/)
[![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/tinde29/telegram-proxy-scraper/issues)
[![Proxy Scraper Workflow](https://github.com/tinde29/telegram-proxy-scraper/actions/workflows/scraper.yml/badge.svg)](https://github.com/tinde29/telegram-proxy-scraper/actions/workflows/scraper.yml)
![GitHub last commit](https://img.shields.io/github/last-commit/tinde29/telegram-proxy-scraper)
![GitHub issues](https://img.shields.io/github/issues/tinde29/telegram-proxy-scraper)

**آخرین به‌روزرسانی پروکسی‌ها**: 22 July 2025, 03:53 UTC (به وقت ایران: 07:23)

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
| 1 | soos-turk.nuremborg-hamborg.dodos-codam.jojo19.ir | 443 | فعال | `tg://proxy?server=soos-turk.nuremborg-hamborg.dodos-codam.jojo19.ir&port=443&secret=7gD_AA___wD_9VVf______VtZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 2 | 178.130.42.116 | 443 | فعال | `tg://proxy?server=178.130.42.116&port=443&secret=eed77db43ee3721f0fcb40a4ff63b5cd276D656469612E737465616D706F77657265642E636F6D` |
| 3 | 65.108.219.52 | 551 | فعال | `tg://proxy?server=65.108.219.52&port=551&secret=79e344818749bd7ac519130220c25d09` |
| 4 | 91.99.231.96 | 155 | فعال | `tg://proxy?server=91.99.231.96&port=155&secret=7hYDAQIAAQAH8AMDhuJMOt1tZWRpYS5zdGVhbXBvd2VyZWQuY29tbWVkaWEuc3RlYW1wb3dlcmVkLmNvbQ` |
| 5 | startup-active.custome-tobano.405bazi.ir | 8888 | فعال | `tg://proxy?server=startup-active.custome-tobano.405bazi.ir&port=8888&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 6 | 49.12.38.200 | 155 | فعال | `tg://proxy?server=49.12.38.200&port=155&secret=dd1603010200010001fc030386e24c3add|[پروکسی](tg://proxy?server=62.60.178.253` |
| 7 | 176.65.128.142 | 8888 | فعال | `tg://proxy?server=176.65.128.142&port=8888&secret=1603010200010001fc030386e24c3add` |
| 8 | 91.99.228.230 | 59065 | فعال | `tg://proxy?server=91.99.228.230&port=59065&secret=eed77db43ee3721f0fcb40a4ff63b5cd276D656469612E737465616D706F77657265642E636F6D` |
| 9 | Focos-mokos.berlino-landcvixo.yokohama-1borino.eromatic.info. | 443 | فعال | `tg://proxy?server=Focos-mokos.berlino-landcvixo.yokohama-1borino.eromatic.info.&port=443&secret=iORid5lJ237IiBMGYMQMdw==` |
| 10 | 62.84.101.60 | 443000 | فعال | `tg://proxy?server=62.84.101.60&port=443000&secret=7hYDAQIAAQAH8AMDhuJMOt1tZWRpYS5zdGVhbXBvd2VyZWQuY29tbWVkaWEuc3RlYW1wb3dlcmVkLmNvbQ` |
| 11 | 2.dfff.cloudflare.com.nokia.com.co.uk.do_yo.want_to.clash_with.this.www.microsoft.com.there_is_no.place_like.localhost.www.bing.com.count_with_me.cyou.net.digikala.com.www.enamad.ir.www.google.com.again_to_fight.everyone.i_am.the_internet.zban-df.info | 8888 | فعال | `tg://proxy?server=2.dfff.cloudflare.com.nokia.com.co.uk.do_yo.want_to.clash_with.this.www.microsoft.com.there_is_no.place_like.localhost.www.bing.com.count_with_me.cyou.net.digikala.com.www.enamad.ir.www.google.com.again_to_fight.everyone.i_am.the_internet.zban-df.info&port=8888&secret=FgMBAgABAAH8AwOG4kw63Q` |
| 12 | www.hihim.sbs | 888 | فعال | `tg://proxy?server=www.hihim.sbs&port=888&secret=ee0c30628212cbbd7ac519130205525d1569612e737465616d706f77657265642e636f6d)__` |
| 13 | 138.199.169.156 | 8888 | فعال | `tg://proxy?server=138.199.169.156&port=8888&secret=FgMBAgABAAH8AwOG4kw63Q` |
| 14 | 46.62.146.42 | 81 | فعال | `tg://proxy?server=46.62.146.42&port=81&secret=7h-Bh5mj0cvgWJcdCXesuLZtZWRpYS5zdGVhbXBvd2VyZWQuY29t)__` |
| 15 | 65.108.12.153 | 65 | فعال | `tg://proxy?server=65.108.12.153&port=65&secret=d77db43ee3721f0fcb40a4ff63b5cd27` |
| 16 | 157.180.120.198 | 888 | فعال | `tg://proxy?server=157.180.120.198&port=888&secret=eeNEgYdJvXrFGRMCIMJdCQ` |
| 17 | 151.244.50.9 | 70 | فعال | `tg://proxy?server=151.244.50.9&port=70&secret=ee0000f00f0f775555fffffff5006e2e696D656469612E737465616D706F77657265642E636F6D` |
| 18 | 157.90.65.125 | 443 | فعال | `tg://proxy?server=157.90.65.125&port=443&secret=7gffffffff_f_Adkb3dubG9hZC53aW5kb3dzdXBkYXRlLmNvbQ` |
| 19 | 88.210.14.179 | 443000 | فعال | `tg://proxy?server=88.210.14.179&port=443000&secret=7hYDAQIAAQAH8AMDhuJMOt1tZWRpYS5zdGVhbXBvd2VyZWQuY29tbWVkaWEuc3RlYW1wb3dlcmVkLmNvbQ` |
| 20 | 91.99.85.639l.ir | 110 | فعال | `tg://proxy?server=91.99.85.639l.ir&port=110&secret=7gAA8A8Pd1VV____9QBuLmktLXcuZ28tLS0=` |
| 21 | 62.60.178.3 | 8888 | فعال | `tg://proxy?server=62.60.178.3&port=8888&secret=7gAA8A8Pd1VV9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t____` |
| 22 | 204.76.203.84 | 443 | فعال | `tg://proxy?server=204.76.203.84&port=443&secret=15115115115115115115115115115115` |
| 23 | 87.248.132.76 | 200 | فعال | `tg://proxy?server=87.248.132.76&port=200&secret=7nngAAAAAAAAAAAAAAAAAABodHRwczovL2FsaWJhYmEuaXI=)__` |
| 24 | 91.99.238.130 | 8080 | فعال | `tg://proxy?server=91.99.238.130&port=8080&secret=7gAA8A8Pd1VV____9QBuLmktLXd3LmZvLS0=` |
| 25 | asd.homayoon19.ir | 155 | فعال | `tg://proxy?server=asd.homayoon19.ir&port=155&secret=eeNEgYdJvXrFGRMCIMJdCQ` |
| 26 | cd9ffdcd077ba605.bytezs.ir | 443 | فعال | `tg://proxy?server=cd9ffdcd077ba605.bytezs.ir&port=443&secret=7gcgcgcgcgcgcgcgcgcgcgd0cmFuc2xhdGUuZ29v)__` |
| 27 | 103.35.189.118 | 8888 | فعال | `tg://proxy?server=103.35.189.118&port=8888&secret=eed0d6e111bada5511fcce9584deadbeef6170706c652e636f6d**` |
| 28 | 213.176.92.143 | 443 | فعال | `tg://proxy?server=213.176.92.143&port=443&secret=eed77db43ee3721f0fcb40a4ff63b5cd276d656469612e737465616d706f77657265642e636f6d` |
| 29 | 87.248.132.42 | 200 | فعال | `tg://proxy?server=87.248.132.42&port=200&secret=eed77db43ee3721f0fcb40a4ff63b5cd276D656469612E737465616D706F77657265642E636F6D` |
| 30 | 94.130.54.26 | 3443 | فعال | `tg://proxy?server=94.130.54.26&port=3443&secret=DDBighLLvXrFGRMCBVJdFQ==` |


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
