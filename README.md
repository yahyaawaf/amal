# قدراتي — نسخة GitHub Pages المصححة

هذه نسخة ثابتة للنشر على GitHub Pages، بدون Supabase أو Cloudflare أو Wrangler أو API خلفي.

## طريقة النشر

1. احذفي ملفات النسخة السابقة من المستودع، وخصوصًا أي Workflow قديم داخل `.github/workflows/`.
2. ارفعي **محتويات هذا المجلد مباشرة** إلى جذر المستودع في الفرع `main`.
3. من **Settings → Pages → Build and deployment** اختاري **GitHub Actions**.
4. افتحي **Actions → Deploy GitHub Pages**.
5. يجب أن تنجح مرحلتا `build` و`deploy`.

## مهم

- لا ترفعي `node_modules` أو `.env.local`.
- لا تضيفي Workflow آخر للنشر بجانب `.github/workflows/pages.yml`.
- ملفات PDF الفعلية توضع داخل `public/files/` بالأسماء المذكورة في `README-PDF.txt`.
- يدعم Workflow تلقائيًا مستودع `username.github.io` أو مشروعًا مثل `username.github.io/amal`.
