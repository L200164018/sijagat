# SIJAGAT Web Wrapper (Vercel)

Web wrapper responsif layar penuh untuk aplikasi AppSheet:
`https://www.appsheet.com/start/2232a87e-c956-4ff9-b9ed-764443e033aa`

Dengan konfigurasi ini, URL peramban tetap berada di domain Anda (`sijagat.vercel.app`) menggunakan iFrame.

## Struktur File

- `index.html`: Wrapper iFrame responsif layar penuh dengan izin akses kamera, mikrofon, dan lokasi untuk fitur AppSheet.
- `vercel.json`: Konfigurasi rute Vercel untuk mengarahkan permintaan ke `index.html`.

## Catatan Penting

- Opsi **Allow app embedding** pada pengaturan aplikasi AppSheet harus selalu dalam kondisi aktif (ON) agar iFrame dapat dimuat.
