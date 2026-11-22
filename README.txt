GULO v2.0 — WINDOWS CMD EDITION
GERAKAN UMKM LOKAL (GULO)
Developed by GFLM

KEBUTUHAN
- Windows 10 atau Windows 11
- Python 3.10 atau lebih baru
- Google Chrome, Microsoft Edge, atau browser modern
- Tidak membutuhkan paket Python pihak ketiga

INSTALASI DARI CMD
1. Ekstrak seluruh isi ZIP ke folder, misalnya C:\GULO.
2. Pasang Python 3.10+ dari https://www.python.org/downloads/windows/.
   Saat instalasi, centang "Add Python to PATH".
3. Buka Command Prompt (CMD).
4. Jalankan:
   cd /d C:\GULO
   setup_windows.bat
5. Setelah setup selesai, jalankan:
   start_gulo.bat
6. Browser membuka http://127.0.0.1:8000.
7. Pada halaman login pilih jenis akun Administrator.

AKUN ADMINISTRATOR PAKET INI
Username: Grazio
Password: WTBSU230107@#
Role: Administrator (akses penuh, tanpa lisensi)

JIKA LOGIN ADMIN TIDAK BERHASIL
1. Hentikan server dari jendela GULO Server dengan Ctrl+C.
2. Pastikan CMD berada pada folder yang sama dengan server.py dan gulo.db.
3. Jalankan:
   reset_admin_password.bat
4. Ketika diminta username admin, tekan Enter untuk memakai grazio atau ketik Grazio.
5. Masukkan password baru dua kali. Input password tidak ditampilkan saat diketik; ini normal.
6. Jalankan kembali:
   start_gulo.bat

PENTING TENTANG DATABASE
- Database aktif adalah file gulo.db di folder aplikasi yang sama dengan server.py.
- File gulo.db pada paket ini sudah berisi akun admin Grazio dengan password di atas.
- Reset password membuat backup database otomatis sebelum mengubah password.
- Jika Anda sudah memiliki database pelanggan dari instalasi sebelumnya, buat backup lalu gunakan database lama pada folder rilis ini sebelum menjalankan reset_admin_password.bat. Jangan menimpa database pelanggan dengan database contoh dalam ZIP.
- Jangan memindahkan server.py tanpa gulo.db.

PERINTAH CMD RINGKAS
cd /d C:\GULO
setup_windows.bat
start_gulo.bat
reset_admin_password.bat

MENGHENTIKAN SERVER
Tekan Ctrl+C pada jendela CMD berjudul "GULO Server - jangan ditutup".

CATATAN KEAMANAN
- Jangan membagikan gulo.db atau backup database karena berisi data akun pelanggan.
- Server default hanya mendengarkan 127.0.0.1 (komputer lokal).
- Untuk penggunaan internet/multi-cabang, diperlukan deployment server dengan HTTPS, backup, dan pengamanan tambahan.
- Akun Administrator tidak memerlukan lisensi; akun UKM memerlukan persetujuan admin dan lisensi aktif.
