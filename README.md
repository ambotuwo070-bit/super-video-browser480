# Super Video Browser

Proyek Android WebView sederhana dengan:
- Kolom alamat dan pencarian Google
- Tombol kembali, maju, beranda, dan muat ulang
- Pengunduhan tautan file/video langsung melalui Download Manager Android
- Pemblokiran dasar beberapa domain iklan/pelacak

## Membuat APK dari HP menggunakan GitHub

1. Buat atau buka repository GitHub `super-video-browser`.
2. Unggah semua isi folder proyek ini ke root repository (bukan folder ZIP-nya).
3. Pastikan file workflow berada di `.github/workflows/build-apk.yml`.
4. Buka tab **Actions** di repository.
5. Pilih **Build Super Video Browser APK**, lalu tekan **Run workflow** (atau tunggu build otomatis setelah push).
6. Setelah selesai, buka hasil workflow dan unduh artifact `Super-Video-Browser-APK`.
7. Ekstrak ZIP artifact, lalu pasang `app-debug.apk` di Android. Izinkan pemasangan dari sumber tersebut bila diminta.

## Batasan penting

Aplikasi ini mengunduh file/video hanya jika situs memberikan tautan unduhan langsung yang dapat diakses WebView. Aplikasi tidak mengekstrak video dari streaming HLS/DASH, tidak melewati DRM, login, paywall, atau pembatasan situs. Pilihan 480p/720p hanya tersedia jika situs menyediakan kualitas tersebut.

Pemblokiran iklan masih dasar dan tidak menjamin semua iklan/pop-up terblokir. Jangan gunakan untuk mengunduh konten yang tidak Anda miliki atau tidak diizinkan untuk diunduh.
