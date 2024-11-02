# High_School_Project

Go to Releases Page

For SHIMA and EXAMBROWSER

# README.md

## Masalah: Error "Display over other apps Feature Not Available" di Smartphone Android

Teman Anda baru-baru ini membeli smartphone Samsung Galaxy dengan anggaran rendah dan saat mencoba menginstal aplikasi, dia menerima pesan error berikut di layar penuh:

**Display over other apps**  
**Feature not available**  
**This feature has been turned off because it slows down your phone.**

Dia mencoba menginstal aplikasi pengunci orang tua atau aplikasi kunci untuk membatasi aplikasi di smartphone-nya, tetapi setiap kali menginstal aplikasi seperti AppLock dari SpSoft, Norton App Lock, dan lainnya, selalu gagal dengan pesan error tersebut.

### Penyebab: Fungsionalitas Screen Overlays Dinonaktifkan oleh Pabrikan Smartphone

Pesan error ini muncul karena fitur "Display over other apps" (juga dikenal sebagai "Draw over other apps" atau "Appear on Top") dinonaktifkan. Fitur ini memungkinkan aplikasi pihak ketiga muncul di atas aplikasi lain, dan sering kali dibatasi untuk aplikasi sistem demi keamanan pengguna.

Pabrikan smartphone sering menonaktifkan fitur ini pada smartphone anggaran untuk meningkatkan performa, mengingat fitur ini dapat mengonsumsi banyak CPU dan RAM.

### Solusi

#### Solusi 1: Mengaktifkan Izin Display Over Other Apps Secara Manual

1. Buka layar utama atau layar peluncur aplikasi.
2. Tekan dan tahan ikon aplikasi untuk membuka menu.
3. Ketuk ikon Info (i) di sudut kanan atas.
4. Cari opsi "Appear on Top" atau "Display over other apps".
5. Jika ada, aktifkan toggle menjadi ON.

#### Solusi 2: Mengaktifkan Pengaturan Screen Overlays Menggunakan Developer Options

1. Aktifkan Developer Options dengan membuka **Settings > About phone > Build number** sebanyak 7 kali.
2. Masuk ke **Developer Options**.
3. Cari opsi "Allow screen overlays" dan aktifkan.

#### Solusi 3: Mengaktifkan Izin Appear on Top Menggunakan Special Access

1. Buka **Settings** dan ketik "Special Access" di kotak pencarian.
2. Pilih opsi Special Access.
3. Pilih "Appear on Top" dan aktifkan toggle untuk aplikasi yang bermasalah.

#### Solusi 4: Memberikan Izin SYSTEM_ALERT_WINDOW Menggunakan ADB Command

1. Unduh dan instal **ADB** (Android Debug Bridge) di PC Anda.
2. Aktifkan USB debugging di smartphone melalui **Developer Options**.
3. Hubungkan smartphone ke PC dan buka Command Prompt di folder Platform-Tools.
4. Jalankan perintah `adb devices` untuk memeriksa koneksi.
5. Temukan nama paket aplikasi di URL Play Store.
6. Jalankan perintah berikut :

   ```
   adb shell pm grant shima.kartinisoft.exambro android.permission.SYSTEM_ALERT_WINDOW
   ```

### Catatan Tambahan

Jika semua langkah di atas gagal, pertimbangkan untuk menggunakan aplikasi alternatif yang tidak memerlukan fitur overlay, atau periksa pembaruan perangkat lunak yang mungkin memperbaiki masalah ini.

Dengan mengikuti langkah-langkah ini, Anda seharusnya dapat mengatasi masalah "Display over other apps feature not available" dan menggunakan aplikasi yang diinginkan.
