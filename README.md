# LeadTrack CRM — halaman web (GitHub Pages)

Halaman pembungkus yang menampilkan aplikasi LeadTrack CRM (Google Apps Script) penuh satu layar di domain **lead-track-crm.my.id**.

| File | Fungsi |
|---|---|
| `index.html` | Menampilkan aplikasi (iframe ke URL `/exec` Apps Script) + animasi loading |
| `CNAME` | Domain kustom: `lead-track-crm.my.id` |
| `logo.png`, `favicon.png`, `apple-touch-icon.png` | Logo, ikon tab browser, ikon saat disimpan ke layar HP |

## Kapan file ini perlu diubah?

- **Update fitur aplikasi** → TIDAK perlu. Cukup di Apps Script: Terapkan → Kelola deployment → ✏️ → Versi baru → Terapkan.
- **Membuat deployment Apps Script BARU** (URL `/exec` berubah) → ganti URL di `index.html`, lalu:

```
git add .
git commit -m "Ganti URL Apps Script"
git push
```
