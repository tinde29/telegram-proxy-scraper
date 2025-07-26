# Telegram Proxy Scraper

[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Python](https://img.shields.io/badge/python-3.9-blue)](https://www.python.org/downloads/)
[![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/tinde29/telegram-proxy-scraper/issues)
[![Proxy Scraper Workflow](https://github.com/tinde29/telegram-proxy-scraper/actions/workflows/scraper.yml/badge.svg)](https://github.com/tinde29/telegram-proxy-scraper/actions/workflows/scraper.yml)
![GitHub last commit](https://img.shields.io/github/last-commit/tinde29/telegram-proxy-scraper)
![GitHub issues](https://img.shields.io/github/issues/tinde29/telegram-proxy-scraper)

**آخرین به‌روزرسانی پروکسی‌ها**: 26 July 2025, 18:56 UTC (به وقت ایران: 22:26)

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
| 1 | xadip.bambo.oooooooooo.ir | 443 | فعال | `tg://proxy?server=xadip.bambo.oooooooooo.ir&port=443&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 2 | Team.hafthashtgswreqetdgsrwrpi-esoiiisolfnwfsksjvwu-urishklfduiwoehv.info. | 6773 | فعال | `tg://proxy?server=Team.hafthashtgswreqetdgsrwrpi-esoiiisolfnwfsksjvwu-urishklfduiwoehv.info.&port=6773&secret=eeNEgYdJvXrFGRMCIMJdCQtY2RueWVrdGFuZXQuY29tZmFyYWthdi5jb212YW4ubmFqdmEuY29tAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA**` |
| 3 | 65.109.193.216 | 443 | فعال | `tg://proxy?server=65.109.193.216&port=443&secret=eeNEgYdJvXrFGRMCIMJdCQ` |
| 4 | 116.202.83.159 | 404 | فعال | `tg://proxy?server=116.202.83.159&port=404&secret=eeNEgYdJvXrFGRMCIMJdCQ` |
| 5 | ownership-nothing-found.enable-request.co.uk | 9741 | فعال | `tg://proxy?server=ownership-nothing-found.enable-request.co.uk&port=9741&secret=ee0000f00f0f775555fffffff5006e2e696d656469612e737465616d706f77657265642e636f6d)__` |
| 6 | 66933.meli.zban-mas.info | 8888 | فعال | `tg://proxy?server=66933.meli.zban-mas.info&port=8888&secret=7gAA8A8Pd1VV____9QBuLmltZWRpYS5zdGVhbXBvd2VyZWQuY29t` |
| 7 | newvip.abineirn2.ir | 70 | فعال | `tg://proxy?server=newvip.abineirn2.ir&port=70&secret=eed77db43ee3721f0fcb40a4ff63b5cd276d656469612e737465616d706f77657265642e636f6d` |
| 8 | 157.180.112.182 | 8888 | فعال | `tg://proxy?server=157.180.112.182&port=8888&secret=1603010200010001fc030386e24c3add` |
| 9 | vip.oliverpro.sbs | 8090 | فعال | `tg://proxy?server=vip.oliverpro.sbs&port=8090&secret=7twxtqyl4JpeItFZJ3sySvJzMy5hbWF6b25hd3MuY29t` |
| 10 | 87.248.132.177 | 200 | فعال | `tg://proxy?server=87.248.132.177&port=200&secret=eeNEgYdJvXrFGRMCIMJdCQ` |
| 11 | 89.251.10.21 | 443 | فعال | `tg://proxy?server=89.251.10.21&port=443&secret=ee151151151151151151151151151151156d656469612e737465616d706f77657265642e636f6d)__` |
| 12 | 10.e7777.cloudflare.com.nokia.com.co.uk.do_yo.want_to.clash_with.this.www.microsoft.com.there_is_no.place_like.localhost.www.bing.com.count_with_me.cyou.net.digikala.com.www.enamad.ir.www.google.com.again_to_fight.everyone.i_am.zban-mas.info | 8888 | فعال | `tg://proxy?server=10.e7777.cloudflare.com.nokia.com.co.uk.do_yo.want_to.clash_with.this.www.microsoft.com.there_is_no.place_like.localhost.www.bing.com.count_with_me.cyou.net.digikala.com.www.enamad.ir.www.google.com.again_to_fight.everyone.i_am.zban-mas.info&port=8888&secret=FgMBAgABAAH8AwOG4kw63Q**` |
| 13 | 45.153.33.19 | 443 | فعال | `tg://proxy?server=45.153.33.19&port=443&secret=7gffffffff_f_Adkb3dubG9hZC53aW5kb3dzdXBkYXRlLmNvbQ` |
| 14 | 157.180.61.201 | 1080 | فعال | `tg://proxy?server=157.180.61.201&port=1080&secret=1320PuNyHw_LQKT_Y7XNJw` |
| 15 | nazanin.212.8-58-185.ir | 443 | فعال | `tg://proxy?server=nazanin.212.8-58-185.ir&port=443&secret=1320PuNyHw_LQKT_Y7XNJw==` |
| 16 | 195.26.226.30 | 443 | فعال | `tg://proxy?server=195.26.226.30&port=443&secret=1320PuNyHw_LQKT_Y7XNJw` |
| 17 | 49.13.145.84 | 443 | فعال | `tg://proxy?server=49.13.145.84&port=443&secret=3QAAAAAAAAAAAAAAAAAAAAA=` |
| 18 | 108.181.70.27 | 3443 | فعال | `tg://proxy?server=108.181.70.27&port=3443&secret=ee082082082082082082082082082082087472616e736c6174652e676f6f**` |
| 19 | 135.181.86.93 | 155 | فعال | `tg://proxy?server=135.181.86.93&port=155&secret=ee07df7df7df7dffdffc07646f776e6c6f61642e77696e646f77737570646174652e636f6d` |
| 20 | 62.60.178.118 | 443 | فعال | `tg://proxy?server=62.60.178.118&port=443&secret=7hYDAQIAAQAH8AMDhuJMOt1tZWRpYS5zdGVhbXBvd2VyZWQuY29tbWVkaWEuc3RlYW1wb3dlcmVkLmNvbQ)`` |
| 21 | 157.180.80.209 | 443 | فعال | `tg://proxy?server=157.180.80.209&port=443&secret=FgMBAgABAAH8AwOG4kw63Q` |
| 22 | 91.99.162.236 | 70 | فعال | `tg://proxy?server=91.99.162.236&port=70&secret=7gAA8A8Pd1VV____9QBuLmktLXcuZ28tLS0=` |
| 23 | 140.233.187.135 | 343 | فعال | `tg://proxy?server=140.233.187.135&port=343&secret=eed77db43ee3721f0fcb40a4ff63b5cd276D656469612E737465616D706F77657265642E636F6D` |
| 24 | bmw.hezarsh-mashal0.co.vjhkgttrrhks-sdcj.co.uk.pwkxjjrhks-skci.co.uk.pwkxjjrhks-ikcj.co.uk.fskxjjrhks-rkcr.co.uk.mstukxjjrhkss-jscj.co.uk. | 7443 | فعال | `tg://proxy?server=bmw.hezarsh-mashal0.co.vjhkgttrrhks-sdcj.co.uk.pwkxjjrhks-skci.co.uk.pwkxjjrhks-ikcj.co.uk.fskxjjrhks-rkcr.co.uk.mstukxjjrhkss-jscj.co.uk.&port=7443&secret=eeRighJJvXrFGRMCIMJdCQ)**` |
| 25 | 5.dfff.cloudflare.com.nokia.com.co.uk.do_yo.want_to.clash_with.this.www.microsoft.com.there_is_no.place_like.localhost.www.bing.com.count_with_me.cyou.net.digikala.com.www.enamad.ir.www.google.com.again_to_fight.everyone.i_am.the_internet.zban-df.info | 8888 | فعال | `tg://proxy?server=5.dfff.cloudflare.com.nokia.com.co.uk.do_yo.want_to.clash_with.this.www.microsoft.com.there_is_no.place_like.localhost.www.bing.com.count_with_me.cyou.net.digikala.com.www.enamad.ir.www.google.com.again_to_fight.everyone.i_am.the_internet.zban-df.info&port=8888&secret=FgMBAgABAAH8AwOG4kw63Q` |
| 26 | 157.180.47.224 | 443 | فعال | `tg://proxy?server=157.180.47.224&port=443&secret=1603010200010001fc030386e24c3add` |
| 27 | 95.216.22.207 | 443 | فعال | `tg://proxy?server=95.216.22.207&port=443&secret=iORid5lJ237IiBMGYMQMdw==` |
| 28 | 95.217.77.168 | 443 | فعال | `tg://proxy?server=95.217.77.168&port=443&secret=7HQighJPBNMYVRNB6tdkVw==` |
| 29 | 91.99.85.639l.ir | 110 | فعال | `tg://proxy?server=91.99.85.639l.ir&port=110&secret=7gAA8A8Pd1VV____9QBuLmktLXcuZ28tLS0=)__` |
| 30 | 62.60.179.198 | 343 | فعال | `tg://proxy?server=62.60.179.198&port=343&secret=FgMBAgABAAfwAwOG4kw63Q` |


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
