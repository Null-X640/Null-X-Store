# Null-X-Store

Toko top-up NULL-X — halaman user + dashboard admin (paket, tier harga, FAQ, diskon, transaksi, users).

## Struktur

- `index.html` + `script.js` — halaman user (order, bayar via QRIS/DANA/GoPay)
- `admin.html` + `admin.js` — dashboard admin (kelola paket/tier, FAQ, diskon, transaksi)
- `admin-login.html` — login admin
- `shared-db.js` — lapisan database (Firebase / Google Sheets / lokal)
- `style.css` — tema dark + aksen ungu `#8b5cf6`
- `netlify.toml` — config deploy Netlify (publish `.`, tanpa build command)

## Deploy (Netlify)

Import repo ini → branch `main` → build command kosong → publish directory `.`.

## Catatan admin

Buka `admin-login.html` untuk masuk dashboard. Data tersimpan lokal (`localStorage` key `nx_*`)
dan didorong ke database online kalau `shared-db.js` sudah dikonfigurasi (Firebase / Sheets).
