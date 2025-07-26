# Telegram Proxy Scraper

[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Python](https://img.shields.io/badge/python-3.9-blue)](https://www.python.org/downloads/)
[![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/tinde29/telegram-proxy-scraper/issues)
[![Proxy Scraper Workflow](https://github.com/tinde29/telegram-proxy-scraper/actions/workflows/scraper.yml/badge.svg)](https://github.com/tinde29/telegram-proxy-scraper/actions/workflows/scraper.yml)
![GitHub last commit](https://img.shields.io/github/last-commit/tinde29/telegram-proxy-scraper)
![GitHub issues](https://img.shields.io/github/issues/tinde29/telegram-proxy-scraper)

**آخرین به‌روزرسانی پروکسی‌ها**: 26 July 2025, 06:56 UTC (به وقت ایران: 10:26)

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
| 1 | 87.248.132.59 | 155 | فعال | `tg://proxy?server=87.248.132.59&port=155&secret=eeNEgYdJvXrFGRMCIMJdCQ` |
| 2 | 198.16.107.91 | 443 | فعال | `tg://proxy?server=198.16.107.91&port=443&secret=ee1603010200010001fc030386e24c3add76616e2e6e616a76612e636f6d` |
| 3 | morgh.2p2p.ir | 8080 | فعال | `tg://proxy?server=morgh.2p2p.ir&port=8080&secret=ee66881e6e1e6d1ff6666666616d66aeae686f73746972616e2e636c6f7564` |
| 4 | 91.99.199.235 | 443 | فعال | `tg://proxy?server=91.99.199.235&port=443&secret=eec862057ba49a7ecdf0ad4eb44cd5bb11646f776e6c6f61642e77696e646f77737570646174652e636f6d` |
| 5 | 195.201.58.218 | 155 | فعال | `tg://proxy?server=195.201.58.218&port=155&secret=ee0000f00f0f775555fffffff5006e2e696d656469612e737465616d706f77657265642e636f6d|[پروکسی](tg://proxy?server=49.12.7.170` |
| 6 | 62.60.177.20 | 443 | فعال | `tg://proxy?server=62.60.177.20&port=443&secret=eed77db43ee3721f0fcb40a4ff63b5cd276D656469612E737465616D706F77657265642E636F6D)__` |
| 7 | 157.180.122.194 | 551 | فعال | `tg://proxy?server=157.180.122.194&port=551&secret=79e344818749bd7ac519130220c25d09` |
| 8 | 5.meli.zban-mas.info | 8888 | فعال | `tg://proxy?server=5.meli.zban-mas.info&port=8888&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 9 | 79.172.228.207 | 70 | فعال | `tg://proxy?server=79.172.228.207&port=70&secret=ee0000f00f0f775555fffffff5006e2e696D656469612E737465616D706F77657265642E636F6D` |
| 10 | 62.60.177.142 | 443 | فعال | `tg://proxy?server=62.60.177.142&port=443&secret=7hYDAQIAAQAH8AMDhuJMOt1tZWRpYS5zdGVhbXBvd2VyZWQuY29tbWVkaWEuc3RlYW1wb3dlcmVkLmNvbQ` |
| 11 | yozar.abarwitch.info | 443 | فعال | `tg://proxy?server=yozar.abarwitch.info&port=443&secret=FgMBAgABAAH8AwOG4kw63Q==` |
| 12 | 157.180.46.166 | 8888 | فعال | `tg://proxy?server=157.180.46.166&port=8888&secret=dd1603010200010001fc030386e24c3add` |
| 13 | 4.dfff.cloudflare.com.nokia.com.co.uk.do_yo.want_to.clash_with.this.www.microsoft.com.there_is_no.place_like.localhost.www.bing.com.count_with_me.cyou.net.digikala.com.www.enamad.ir.www.google.com.again_to_fight.everyone.i_am.the_internet.zban-df.info | 8888 | فعال | `tg://proxy?server=4.dfff.cloudflare.com.nokia.com.co.uk.do_yo.want_to.clash_with.this.www.microsoft.com.there_is_no.place_like.localhost.www.bing.com.count_with_me.cyou.net.digikala.com.www.enamad.ir.www.google.com.again_to_fight.everyone.i_am.the_internet.zban-df.info&port=8888&secret=FgMBAgABAAH8AwOG4kw63Q` |
| 14 | 193.3.190.60 | 85 | فعال | `tg://proxy?server=193.3.190.60&port=85&secret=ee0000f00f0f775555fffffff5006e2e696d656469612e737465616d706f77657265642e636f6d` |
| 15 | 157.180.30.251 | 443 | فعال | `tg://proxy?server=157.180.30.251&port=443&secret=iORid5lJ237IiBMGYMQMdw` |
| 16 | 193.3.190.74 | 85 | فعال | `tg://proxy?server=193.3.190.74&port=85&secret=ee0c30628212cbbd7ac519130205525d1569612e737465616d706f77657265642e636f6d` |
| 17 | 62.60.178.33 | 443 | فعال | `tg://proxy?server=62.60.178.33&port=443&secret=7hYDAQIAAQAH8AMDhuJMOt1tZWRpYS5zdGVhbXBvd2VyZWQuY29tbWVkaWEuc3RlYW1wb3dlcmVkLmNvbQ)`` |
| 18 | 5.255.126.224 | 443 | فعال | `tg://proxy?server=5.255.126.224&port=443&secret=7hYDAQIAAQAB_AMDhuJMOt1tZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 19 | 500.meli.zban-mas.info | 8888 | فعال | `tg://proxy?server=500.meli.zban-mas.info&port=8888&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 20 | 87.229.100.237 | 443 | فعال | `tg://proxy?server=87.229.100.237&port=443&secret=eeRighJJvXrFGRMCIMJdCQ` |
| 21 | 91.107.164.77 | 27 | فعال | `tg://proxy?server=91.107.164.77&port=27&secret=1320PuNyHw_LQKT_Y7XNJw==` |
| 22 | 188.245.144.93 | 443 | فعال | `tg://proxy?server=188.245.144.93&port=443&secret=eec862057ba49a7ecdf0ad4eb44cd5bb11646f776e6c6f61642e77696e646f77737570646174652e636f6d` |
| 23 | 47.250.149.86 | 443 | فعال | `tg://proxy?server=47.250.149.86&port=443&secret=ee0d99db994ed1ca453d83df742a2454ac617a7572652e6d6963726f736f66742e636f6d` |
| 24 | 157.180.80.64 | 8888 | فعال | `tg://proxy?server=157.180.80.64&port=8888&secret=FgMBAgABAAH8AwOG4kw63Q` |
| 25 | 62.60.177.56 | 443 | فعال | `tg://proxy?server=62.60.177.56&port=443&secret=7hYDAQIAAQAH8AMDhuJMOt1tZWRpYS5zdGVhbXBvd2VyZWQuY29tbWVkaWEuc3RlYW1wb3dlcmVkLmNvbQ)|` |
| 26 | 62.60.178.146 | 443 | فعال | `tg://proxy?server=62.60.178.146&port=443&secret=7hYDAQIAAQAH8AMDhuJMOt1tZWRpYS5zdGVhbXBvd2VyZWQuY29tbWVkaWEuc3RlYW1wb3dlcmVkLmNvbQ` |
| 27 | 7.1.ir.ir.brobalair.ink | 8888 | فعال | `tg://proxy?server=7.1.ir.ir.brobalair.ink&port=8888&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t)__` |
| 28 | 65.109.170.104 | 100 | فعال | `tg://proxy?server=65.109.170.104&port=100&secret=c862057ba49a7ecdf0ad4eb44cd5bb11` |
| 29 | 98.link-a2.ir | 443 | فعال | `tg://proxy?server=98.link-a2.ir&port=443&secret=eed77db43ee3721f0fcb40a4ff63b5cd276D656469612E737465616D706F77657265642E636F6D` |
| 30 | 157.180.95.47 | 443 | فعال | `tg://proxy?server=157.180.95.47&port=443&secret=eeNEgYdJvXrFGRMCIMJdCQ` |


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
