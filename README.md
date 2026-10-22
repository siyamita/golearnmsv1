# GoLearnMS
Deploy: push ke GitHub → import di Vercel (Framework: Other).
1. Vercel → Storage/Marketplace → tambah **Upstash Redis** (otomatis mengisi KV_REST_API_URL & KV_REST_API_TOKEN).
2. Environment Variables: `AUTH_SECRET` (teks acak panjang), `ANTHROPIC_API_KEY` (Asisten AI), `RESEND_API_KEY` (e-mail reset & chat admin), opsional `MAIL_FROM`, `SITE_URL`.
3. Redeploy. Admin utama: username `siya`, password `12345siya`, kata kunci `a` (segera ganti password!).

## Struktur (jangan diubah)
```
api/app.js        ← backend (Vercel Serverless Function, otomatis jadi /api/app)
public/index.html ← tampilan (frontend) — memanggil /api/app
public/logo.svg
package.json, vercel.json
```
Upload **isi folder** ini ke root repo GitHub (bukan file zip-nya).
