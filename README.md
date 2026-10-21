# أثر — Twilight theme scaffold

تم تحويل التصميم إلى بنية Salla Twilight Legacy/Twig قابلة للربط:

- `twilight.json` يعرّف الميزات والإعدادات ومكوّن الصفحة الرئيسية.
- `src/views/layouts/master.twig` هو التخطيط العام الذي يربط خط وألوان المتجر وhooks سلة.
- `src/views/pages/index.twig` هو مسار الصفحة الرئيسية القياسي.
- `src/views/components/home/athhar-home.twig` يحتوي على تجربة أثر الرئيسية.
- `src/assets/styles/app.css` و`src/assets/js/app.js` للأصول الخاصة بالثيم.

## ما يلزم قبل التشغيل والنشر

1. سجّل الدخول إلى Salla Partners من خلال CLI: `salla login`.
2. اربط المشروع بثيم منشأ من Partners Portal أو استخدم `salla theme create` من نسخة CLI الحديثة.
3. راجع اسم مستودع GitHub والبريد في `twilight.json`.
4. ثبّت الاعتمادات باستخدام `pnpm install` ثم شغّل `salla theme preview` أو أمر المعاينة المدعوم في نسخة CLI لديك.
5. اربط بطاقات المنتجات والمكونات الديناميكية ببيانات المتجر قبل النشر.

هذه الخطوة لا يمكن تنفيذها تلقائياً من البيئة الحالية لأن CLI المثبت يطلب مصادقة Salla والاتصال الخارجي غير متاح، لكنها تترك مصدر الثيم في صورة قابلة للإكمال والربط.
