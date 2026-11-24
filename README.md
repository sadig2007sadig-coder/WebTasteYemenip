# كتابي الذكي – دليل الرفع على GitHub Pages
1. أنشئ مستودعاً جديداً وارفع **كل** الملفات والمجلدات (index.html, style.css, app.js, data.js, config.js, assets/).
2. Settings ← Pages ← Branch: main ← Save. سيعمل الموقع على رابط github.io.

## رمز التحقق إلى البريد (EmailJS – مجاني)
1. سجّل في emailjs.com وأضف Email Service (Gmail مثلاً).
2. أنشئ Template: To email = {{to_email}}، والنص يحتوي: مرحباً {{to_name}}، رمزك {{code}}.
3. انسخ Public Key و Service ID و Template ID إلى config.js.
بدون ذلك يعمل الموقع بوضع تجريبي يعرض الرمز على الشاشة.

## الكتاب المحلول
ضع صوره في assets/solved بأسماء s-01.jpg ... s-82.jpg و cover.jpg. إن لم توجد يعرض الكتاب الأصلي مع تنبيه.

## الأسئلة والنماذج
عدّلها في data.js (كل وحدة 7 أسئلة صح/خطأ واختيار من متعدد، مع شرح عند الخطأ).

## تنبيه أمني
GitHub Pages موقع ثابت بلا خادم؛ الحسابات تُحفظ في متصفح المستخدم (كلمات السر مشفّرة SHA-256) والتحقق يتم في المتصفح.
للأمان الحقيقي (حسابات مشتركة بين الأجهزة وتحقق من الخادم) استخدم Firebase Auth أو Supabase.
