# 🎓 High School Project — Kumpulan APK Proyek Sekolah

Repositori ini berisi kumpulan aplikasi Android (APK) hasil proyek sekolah untuk berbagai kebutuhan pendidikan seperti ujian online, penjadwalan, hingga browser khusus.

---

## 📦 Daftar Aplikasi

* **CBTSMANCAV11.apk** — Aplikasi ujian CBT untuk MAN CAV
* **PBSSI\_JAYA\_BROWSER.apk** — Browser khusus untuk keperluan internal
* **PENJADWALAN\_KERJA\_FINAL.apk** — Aplikasi penjadwalan kerja
* **PRATA\_EXAMBRO.apk** — Browser aman untuk ujian berbasis Android
* **SHIMA\_LAST.apk** — Aplikasi ujian SHIMA

---

## ⚠️ Masalah Umum: "Display over other apps Feature Not Available"

Beberapa pengguna mengalami error saat menjalankan aplikasi yang memerlukan izin overlay:

```
Display over other apps
Feature not available
This feature has been turned off because it slows down your phone.
```

### 🔍 Penyebab

Fitur "Display over other apps" dinonaktifkan oleh produsen smartphone (terutama di perangkat low-end) untuk meningkatkan performa.

---

## 🛠️ Solusi

### 1. Aktifkan Izin Lewat Pengaturan Aplikasi

* Tekan dan tahan ikon aplikasi → Info aplikasi → "Tampil di atas aplikasi lain" → Aktifkan.

### 2. Aktifkan via Developer Options

* Buka `Settings > About phone > tap Build number 7x` → Developer Options → Aktifkan "Allow screen overlays".

### 3. Akses Khusus (Special Access)

* `Settings > Special Access > Appear on Top` → Aktifkan untuk aplikasi terkait.

### 4. Gunakan ADB (Android Debug Bridge)

```bash
adb shell pm grant shima.kartinisoft.exambro android.permission.SYSTEM_ALERT_WINDOW
```

> Pastikan USB Debugging aktif dan ADB sudah terpasang di PC Anda.

---

## 📥 Rilis Terbaru

Lihat rilis: [Python\&CPP.apk](https://github.com/SecretDiscorder/High_School_Project/releases)

---

## 📄 Lisensi

Proyek ini dilisensikan di bawah [GPL-3.0 License](https://www.gnu.org/licenses/gpl-3.0.html).

---

## 👨‍💻 Kontributor

* [SecretDiscorder](https://github.com/SecretDiscorder)
