# Parts Mart — الواجهة (Frontend)

مشروع React حقيقي (Vite + Tailwind)، جاهز للنشر على Vercel أو Netlify.

## البنية
```
parts-mart-frontend/
  index.html
  package.json
  vite.config.js
  tailwind.config.js
  postcss.config.js
  src/
    main.jsx
    App.jsx      ← كل كود التطبيق هنا
    index.css
```

## النشر من الآيفون (بدون كمبيوتر)

### ١. رفع المشروع على GitHub
1. أنشئ مستودعًا جديدًا (مثلاً `parts-mart-frontend`) — نفس طريقة مستودع الخادم.
2. ارفع **كل الملفات والمجلدات** بهيكلها كما هي (احرص أن يبقى `src/App.jsx` داخل مجلد `src`، وليس في الجذر).

### ٢. النشر على Vercel
1. اذهب إلى vercel.com من Safari وسجّل دخول بحساب GitHub نفسه.
2. اضغط "Add New" → "Project".
3. اختر مستودع `parts-mart-frontend`.
4. Vercel سيتعرف تلقائيًا أنه مشروع Vite (بفضل `package.json` و`vite.config.js`) ويملأ إعدادات البناء تلقائيًا:
   - Build Command: `vite build`
   - Output Directory: `dist`
5. اضغط "Deploy" وانتظر دقيقتين تقريبًا.
6. سيعطيك رابطًا مثل: `https://parts-mart-frontend.vercel.app` — هذا رابط تطبيقك النهائي الذي يمكنك مشاركته مع أي شخص.

## ملاحظة مهمة
`src/App.jsx` يتصل بالفعل بخادم Railway المنشور مسبقًا (`API_BASE` في أعلى الملف). لا حاجة لتغيير أي شيء إضافي — بمجرد نشر هذه الواجهة، سيتصل التطبيقان ببعضهما تلقائيًا لأنهما الآن موقعان حقيقيان على الإنترنت وليسا محكومين ببيئة معاينة محدودة.
