# Video 60 fps di YouTube Terasa Patah-patah
Solusi ini dicoba pada
- Fedora Workstation 43
- Firefox 144
## Masalah
Ketika memutar video 60fps, terasa seperti tidak lancar
## Penyebab
Fedora Workstation 43 mengimplementasikan Wayland sebagai protokol komunikasi _display server_. Kebijakan ini sebenernya bukan hal baru namun pada versi sebelumnya pengguna masih dapat menggunakan X.org sedangkan pada versi 43, pengguna hanya dapat menggunakan Wayland.
## Solusi
Agar dapat menonton Youtube dengan lancar, kita akan memaksa browser untuk berjalan menggunakan Xwayland.
1. Pertama-tama pastikan bahwa Firefox versi RPM sudah terinstall di komputer anda. Jika belum, anda dapat mengunduh dengan perintah:
```
$ sudo dnf install firefox
```
2. Verikasi bahwa anda menginstall Firefox versi RPM menggunakan perintah:
```
$ rpm -qa | grep "firefox"
```
3. Jika di bawahnya muncul tulisan seperti ini:
```
firefox-144.0.2-1.fc43.x86_64
firefox-langpacks-144.0.2-1.fc43.x86_64
```
maka selamat, Firefox yang anda miliki adalah versi RPM (catatan, angka yang muncul setelah kata "firefox" adalah versi aplikasi sehingga bukan masalah apabila angka yang muncul di perangkat anda berbeda)

4. Setelah itu, install aplikasi Main Menu menggunakan perintah ini:
```
$ flatpak install flathub page.codeberg.libre_menu_editor.LibreMenuEditor
```
(secara default, Flatpak sudah terinstall di Fedora Workstation)

5. Pada aplikasi Main Menu klik Firefox pada sidebar samping untuk selanjutnya mengedit "Default command" dari `firefox %u` menjadi `env MOZ_ENABLE_WAYLAND=0 firefox %u`
<img width="2100" height="1700" alt="Screenshot From 2025-11-13 21-38-43" src="https://github.com/user-attachments/assets/66bf1fa6-38ae-46f8-9a61-7ece8f0b7942" />

6. Klik save dan buka Firefox.
7. Tulis `about:support` dan arahkan ke "windows protocol"
8. Apabila sudah tertulis `xwayland` pada "windows protocol" seperti gambar di bawah, maka solusi sudah berhasil diterapkan.
<img width="691" height="169" alt="Screenshot From 2025-11-13 21-44-34" src="https://github.com/user-attachments/assets/34a3c8f0-32a2-479f-890d-55878a873697" />

9. Enjoy YouTube 60 fps!
