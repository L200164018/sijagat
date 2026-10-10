# AppSheet URL Shortener (Vercel)

Proyek ini mengalihkan pengunjung dari domain Anda langsung ke aplikasi AppSheet:
`https://www.appsheet.com/start/2232a87e-c956-4ff9-b9ed-764443e033aa`

## Struktur File

- `vercel.json`: Konfigurasi edge redirect Vercel (HTTP 307).
- `index.html`: Cadangan (fallback) dengan meta refresh jika redirect edge tertunda atau dibuka di browser lawas.

## Cara Deploy ke Vercel

### Opsi 1: Menggunakan Vercel CLI

1. Buka terminal di folder ini.
2. Jalankan perintah:
   ```bash
   npx vercel
   ```
3. Ikuti petunjuk di terminal untuk login dan memilih nama project (misalnya `appsheet-pendataan`).
4. Setelah selesai, deploy ke production:
   ```bash
   npx vercel --prod
   ```

### Opsi 2: Menggunakan GitHub

1. Push folder ini ke repository GitHub baru.
2. Buka dashboard [Vercel](https://vercel.com) lalu klik **Add New** > **Project**.
3. Import repository tersebut dan klik **Deploy**.
4. (Opsional) Tambahkan custom domain milik Anda di menu **Settings** > **Domains**.

## Catatan Konfigurasi (`vercel.json`)

- Parameter `"permanent": false` menghasilkan status HTTP 307 (Temporary Redirect). Opsi ini disarankan agar browser tidak meng-cache URL tujuan secara permanen jika sewaktu-waktu link AppSheet Anda berubah.
- Jika ingin redirect disimpan permanen di cache browser (HTTP 308), ubah nilai `"permanent"` menjadi `true`.
