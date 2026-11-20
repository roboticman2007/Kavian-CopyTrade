

bash <(curl -Ls https://raw.githubusercontent.com/roboticman2007/Kavian-CopyTrade/main/install_kaviancopytrade.sh)


نصب روی سرور هتزنر آلمان
فایل install_kaviancopytrade_v1_0.sh رو به مسیر /root/ روی سرور هتزنر آپلود کن:

حالت ۱ — نصب سریع با آی‌پی سرور (برای تست فوری قبل از وصل کردن دامنه):

Bash

sed -i 's/\r$//' /root/install_kaviancopytrade.sh && chmod +x /root/install_kaviancopytrade.sh && bash /root/install_kaviancopytrade.sh

بعد از نصب، سایت روی آدرس http://SERVER_IP:8900 بالا میاد.

حالت ۲ — نصب مستقیم با دامنه و گواهی SSL رایگان (اگر از قبل A Record دامنه رو روی آی‌پی هتزنر گذاشتی):

Bash

sed -i 's/\r$//' /root/install_kaviancopytrade.sh && chmod +x /root/install_kaviancopytrade.sh && bash /root/install_kaviancopytrade.sh copy.yourdomain.com admin@yourdomain.com

اتصال دامنه و SSL در آینده (هر زمان بعد از نصب حالت ۱):

Bash

kavian-copytrade-ssl copy.yourdomain.com admin@yourdomain.com

اطلاعات ورود اولیه و پیشنهاد برای اولین تست بی‌ریسک
ورود مستر ادمین: یوزرنیم admin / پسورد admin12345 (از /admin وارد شو و در اولین فرصت یک کاربر تست بساز).

تست گام‌به‌گام قبل از پول واقعی:

یک اکانت تریدر تست بساز و تاییدش کن؛ به‌صورت پیش‌فرض هر کاربر یک حساب Paper Simulator ($10,000) فعال داره.

با اکانت تریدر وارد /dashboard شو، سوییچ Auto-Trade رو روشن کن و مارجین/اهرم دلخواه رو ذخیره کن.

از کنسول ادمین یک سیگنال تستی (یا یک متن سیگنال تلگرام توی بخش Parser Test) دیسپچ کن تا اجرای موازی، باز شدن پوزیشن، مانیتورینگ زنده و کلوز دستی رو ببینی.

مرحله بعد از داخل اکانت تریدر، کلید Binance Testnet یا Bybit Testnet رو وصل کن و دوباره تست بگیر؛ وقتی همه‌چیز دقیقاً مطابق میلت بود، آماده ورود روی حساب واقعی با مبالغ کم هستی.

نصبش کن و نتیجه اولین تستت رو بگو تا اگر هر بخش (مثلاً تغییر پسورد ادمین از UI، درگاه اشتراک، فارسی‌سازی کامل رابط کاربری یا اتصال مستقیم kaviancrypto به وب‌هوکش) نیاز به ارتقا داشت، همون رو دقیقاً روی پروژه کاویان کپی ترید پیاده کنیم.
