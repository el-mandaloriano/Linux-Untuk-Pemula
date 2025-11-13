# Perkenalan 👋
Panduan ini saya dedikasikan untuk siapapun yang terlanjur hijrah ke Linux. Linux bukan lah ekosistem yang sulit untuk dipelajari namun membutuhkan kerja lebih (extra steps) apalagi jika sudah terbiasa dengan Windows dan Mac OS. Panduan ini merupakan rangkuman dari masalah yang saya hadapi dalam menggunakan Linux. Pada panduan ini saya tidak menyediakan cara menginstall distro Linux.
## Distro apa yang cocok untuk pemula?
Sebenarnya tidak ada distro yang "terbaik". Semua distro adalah baik apabila cocok dengan kebutuhan penggunanya. Jika ada orang yang mengatakan distro a lebih baik dari distro b sebaiknya abaikan saya dan sesuaikan dengan kebutuhan kalian. Walaupun demikian, saya memilih distro Fedora karena kompatibilitasnya dengan perangkat yang saya miliki. Sedikit cerita, saya tidak pernah mengalami masalah dengan driver di distro ini, semua perangkat keras dapat berjalan dengan baik _straight out of the box_.
## Siapa saya? 🧐
Saya bukan seorang programmer, sehingga coding bukan zona yang nyaman saya tempat namun saya adalah pengguna biasa yang "nekat hijrah ke Linux. Alasannya tidak lain tidak bukan adalah semakin agresifnya MS menambahkan fitur Ai pada Windows 11. Saya bukan lah orang yang anti Ai sebab saya juga berlangganan Gemini tetapi saya tidak nyaman jika Ai hadir di setiap sudut ekosistem perangkat. Bagi saya, perangkat adalah barang personal yang harus dihargai privasinya layaknya penggunanya.
## Kenapa membuat panduan ini? 🗒️
Masih sedikitnya _troubleshooters_ yang berbahasa Indonesia yang langsung menuliskan masalah serta solusinya secara spesifik. Jika kalian _browsing_ di mesin pencari, kalian akan menemukan banyak sekali tutorial tentang Linux namun saya kerap kali kesulitan apabila menghadapi masalah yang spesifik seperti kendala pada aplikasi tertentu.
## Apa saja cakupan dari panduan ini? 🔭
Seperti yang sudah saya tulis di atas, panduan ini akan mencakup masalah yang saya hadapi selama menggunakan distro Fedora sehingga apa yang saya tulis di sini tidak akan runut layaknya tutorial. Walapun demikian, panduan ini seharusnya dapat diterapkan pada distro lain dengan sedikit penyesuaian.
## Apakah panduan ini dapat dapat menyelesaikan masalah yang saya hadapi? 🤔
Tentu tidak. Seringkali ditemui ketika suatu software menjalani pembaruan (update), konfigurasi dari versi sebelumnya tidak berjalan di konfigurasi baru. Oleh karena itu, penting bagi saya untuk menuliskan di versi apa solusinya dijalankan. Di sisi lain, terdapat juga situasi di mana sebuah konfigurasi dapat dijalankan di semua versi. Dengan demikian, tidak ada salahnya untuk mencoba solusi yang ditulis pada panduan ini
## Direktori penting
Sebelum melakukan penyelesaikan terhadap masalah, penting bagi kita untuk mengetahui perbedaan aplikasi Flatpak dan RPM. Detail untuk kedua jenis tersebut tidak akan saya bahas di sini namun kedua aplikasi tersebut memiliki perbedaan direktori instalasi:
- Flatpak: `/var/lib/flatpak/app`
- RPM: `/home/username_kamu/.var/app`
## Catatan penting
Daftar masalah pada tulisan ini akan bertambah seiring dengan perjalanan saya menggunakan Fedora. 
## Daftar masalah (per November 2025)
- [Video Youtube patah-patah](Video_patah2.md)
