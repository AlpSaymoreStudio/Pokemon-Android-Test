# Pokemon GBC Android

Android WebView app untuk menjalankan ROM Game Boy atau Game Boy Color yang dipilih dari perangkat pengguna.

## Cara pakai

1. Install APK di Android.
2. Buka aplikasi.
3. Tekan **Pilih ROM dari HP**.
4. Pilih file `.gb` atau `.gbc` yang kamu miliki secara legal.

## Build APK otomatis

Setiap push ke branch `main` atau `master` menjalankan GitHub Actions:

1. Menyiapkan JDK 17 dan Gradle 8.4.
2. Build debug APK.
3. Upload APK sebagai workflow artifact.
4. Membuat GitHub Release berisi APK saat push ke branch utama.

Download APK dari tab **Actions** atau **Releases** di GitHub.

## Build lokal

```bash
gradle assembleDebug
```

APK akan berada di:

```text
app/build/outputs/apk/debug/
```

ROM tidak disertakan di repo ini. Gunakan hanya file ROM yang kamu miliki haknya.
