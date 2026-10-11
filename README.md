# SIJAGAT URL Shortener (Vercel)

Pengalihan tautan resmi untuk aplikasi AppSheet:

1. **Domain Utama (`sijagat.my.id` & `www.sijagat.my.id`)**:
   Mengarahkan ke halaman aplikasi utama:
   `https://www.appsheet.com/start/2232a87e-c956-4ff9-b9ed-764443e033aa`

2. **Subdomain Mobile (`mobile.sijagat.my.id`)**:
   Mengarahkan langsung ke shortcut instalasi mobile:
   `https://www.appsheet.com/newshortcut/2232a87e-c956-4ff9-b9ed-764443e033aa`

## Konfigurasi DNS

- **Domain Utama**: Tipe `A`, Name `@`, Value `76.76.21.21`
- **Subdomain WWW**: Tipe `CNAME`, Name `www`, Value `cname.vercel-dns.com`
- **Subdomain Mobile**: Tipe `CNAME`, Name `mobile`, Value `cname.vercel-dns.com`
