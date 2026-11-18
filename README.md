# রান্না শিখুন — Android WebView অ্যাপ

ওয়েবসাইট: https://rannashikhun.github.io/Cooking/

## APK বানানোর নিয়ম (Android Studio)
1. Android Studio (Koala বা নতুন) খুলুন → **Open** → এই `RannaShikhunApp` ফোল্ডারটি সিলেক্ট করুন।
2. Gradle Sync শেষ হওয়া পর্যন্ত অপেক্ষা করুন (ইন্টারনেট লাগবে)।
3. টেস্ট APK: **Build → Build APK(s)** → `app/build/outputs/apk/debug/app-debug.apk`
4. Play Store / রিলিজের জন্য: **Build → Generate Signed Bundle / APK** দিয়ে নিজের keystore দিয়ে সাইন করুন।

## কাস্টমাইজ
- সাইটের লিংক: `MainActivity.kt` এর `homeUrl` ও `siteHost`
- রং: `app/src/main/res/values/colors.xml` (`primary`)
- অ্যাপের নাম: `res/values/strings.xml`
- আইকন: `res/drawable/ic_launcher_foreground.xml` (নিজের লোগো দিতে Android Studio → New → Image Asset)
- প্যাকেজ নাম: `com.rannashikhun.app` (Play Store-এ দিলে নিজের নাম দিন)

## ফিচার
- পুরো স্ক্রিন অ্যাপের মতো (অ্যাড্রেস বার নেই)
- উপরে লোডিং বার, টেনে রিফ্রেশ (pull-to-refresh)
- ব্যাক বাটনে পেজের পেছনে যায়, শেষে অ্যাপ বন্ধ হয়
- অন্য সাইটের লিংক ফোনের ব্রাউজারে খোলে
- ইন্টারনেট না থাকলে বাংলা এরর স্ক্রিন + আবার চেষ্টা বাটন
- ফুলস্ক্রিন ভিডিও ও ফাইল/ছবি আপলোড সাপোর্ট
