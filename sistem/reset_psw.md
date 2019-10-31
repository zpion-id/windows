## RESET PASSWORD WINDOWS 10 DENGAN chntpw di UBUNTU 18.04

#### Tahap Persiapan
1. Shutdown windows dengan menekan dan menahan tombol shift+shutdown
2. Download Ubuntu desktop 18.04 dan buat bootable USB.
3. download `chntpw` di https://ubuntu.pkgs.org/18.04/ubuntu-universe-i386/chntpw_1.0-1build1_i386.deb.html
4. Restart PC dan tekan F12 untuk boot menu.
5. Pilih boot dari flash disk yang sudah di pasang ubuntu 18.04
6. Install chntpw yang sudah di download di atas dengan mengetik `sudo dpkg -i chntpw_1.0-1build1_i386.deb`
7. Jika sudah di install pastikan `chntpw` berjalan dengan cara ketik `chntpw` di terminal

#### Tahap Reset
1. Masuk ke direktori `Windows\System32\Config\
2. Periksa daftar username yang tersedia dengan mengetik `chntpw -l SAM`
3. Pilih username yang mau direset dengan cara ketik `chntpw -u User_name SAM`
4. Untuk reset (blank) password pilih nomor 1.
5. Jika sudah selesai pilih `q` dan ketik `y`.
6. Selesai silahkan login dengan user yang telah direset dan tanpa password.
