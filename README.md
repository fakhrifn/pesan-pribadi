# Pesan Pribadi

WhatsApp Web versi sendiri yang berjalan sebagai **aplikasi di PC Windows Anda**. Chat, sesi login,
dan media tersimpan di komputer Anda — tidak ada server perantara.

**Unduh:** [Rilis terbaru](../../releases/latest) → `Pesan-Pribadi-Setup-<versi>.exe`
· Halaman lengkap: https://portofolio-fakhri-dev.web.app/pesan-pribadi.html

## Kenapa lebih pribadi

- **Berjalan di PC Anda sendiri** — bukan di server kami. Tanpa akun, tanpa pendaftaran.
- **Chat & memori 100% di PC Anda** — sesi, chat, foto, dan pesan suara disimpan di folder aplikasinya.
- **Kami tidak menyimpan apa pun** — tanpa analitik dan pelacak; aplikasinya hanya terhubung ke server WhatsApp.
- **Hanya PC Anda yang bisa membukanya** — server lokalnya hanya menerima akses dari `127.0.0.1`;
  permintaan dari jaringan lain atau situs web lain ditolak.
- **Privasi di layar** — buram pesan, tirai chat, kunci PIN, dan tanpa centang biru.

## Memasang

1. Unduh `Pesan-Pribadi-Setup-<versi>.exe` dari [Rilis](../../releases/latest) (±47 MB, Node.js sudah termasuk).
2. Jalankan. Muncul *"Windows melindungi PC Anda"*? Klik **Info selengkapnya → Tetap jalankan** —
   peringatan itu muncul karena aplikasinya belum ditandatangani sertifikat berbayar. Tanpa hak admin.
3. Atur privasi & PIN, lalu scan kode QR dari HP: WhatsApp → **Perangkat tertaut** → **Tautkan perangkat**.

**Cek keaslian berkas:** di Command Prompt jalankan
`certutil -hashfile Pesan-Pribadi-Setup-<versi>.exe SHA256`, lalu cocokkan dengan SHA-256 di catatan rilis.

**Menghapus:** Pengaturan Windows → Aplikasi → Pesan Pribadi → Uninstall. Chat & sesi hanya ikut
terhapus bila Anda mencentangnya. Keluarkan dulu perangkat ini dari HP lewat Perangkat tertaut.

## Yang perlu Anda tahu

- **Bukan aplikasi resmi WhatsApp.** Dibangun di atas [Baileys](https://github.com/WhiskeySockets/Baileys),
  pustaka sumber terbuka yang tidak resmi. Untuk pemakaian pribadi risikonya kecil, tapi tidak nol.
- Riwayat chat lama tidak diambil — hanya pesan sejak perangkat ditautkan.
- PIN & buram melindungi tampilan, bukan enkripsi berkas.
- PC harus menyala agar pesan masuk. Saat ini khusus Windows 10/11 64-bit.

---

**English:** Pesan Pribadi is a personal WhatsApp Web client that runs as a Windows app on your own PC.
Chats and your session stay on your computer; its local server only accepts connections from `127.0.0.1`,
and the app only connects to WhatsApp's servers. Download the installer from
[Releases](../../releases/latest) (Windows 10/11, 64-bit). Built on the unofficial Baileys library.

*Pesan Pribadi adalah proyek independen dan tidak berafiliasi dengan, didukung, atau disponsori oleh
WhatsApp LLC maupun Meta Platforms, Inc. WhatsApp adalah merek dagang milik Meta Platforms, Inc.*
