![Marcellyno · Developer Cartridge](./pixel-banner.svg)

`PLAYER 01 / MARCELLYNO` &nbsp; `SAVE FILE / INFORMATIKA`

> Di Unity, saya bisa bikin kota yang enak dilihat tapi masih terasa kosong. Di WhatsApp, saya bisa bikin agent yang jawabannya meyakinkan tapi belum tentu mencatat pesanan yang benar. Saya suka bagian setelah prototipe pertama jadi: mencari tahu **apa yang masih gagal**, lalu memperbaikinya.

## Select a world

**[01 · AI Lab](#01-ai-lab)** &nbsp; **[02 · Game Studio](#02-game-studio)** &nbsp; **[03 · Systems Deck](#03-systems-deck)** &nbsp; **[04 · Repo Vault](#04-repo-vault)**

## 01 AI Lab

### Kalau pelanggan bilang “eh, ganti jadi tiga”?

Saya membangun prototipe agent pemesanan WhatsApp dengan **Google ADK** untuk skripsi. Contoh berikut menunjukkan keputusan desain yang penting: kalau detail pesanan berubah, persetujuan atas ringkasan lama tidak ikut berlaku.

<details>
<summary><b>A ▸ Pelanggan setuju dengan ringkasan</b></summary>

Agent bisa melanjutkan alur dengan rincian yang disetujui. Dalam penelitian saya, yang dicek adalah **tindakan yang dipilih agent dan hasil pencatatannya**, bukan sekadar apakah balasannya terdengar natural.

</details>

<details>
<summary><b>B ▸ Pelanggan mengubah jumlah</b></summary>

Ringkasan lama tidak lagi cocok. Agent perlu memperbaruinya dan meminta persetujuan atas rincian yang baru. Kalau isi chat terlihat benar tapi yang tercatat masih jumlah lama, skenario itu tetap gagal.

</details>

## 02 Game Studio

### TOU / Kota yang masih terasa kosong

**Save point:** Di prototipe Unity, saya sudah mengiterasi pencahayaan, material, dan lingkungan. Tampilan kotanya mulai saya suka, tapi lensa berikutnya adalah pengalaman berjalan di dalamnya: apa yang menarik perhatian, ke mana pemain ingin belok, dan pintu mana yang pantas bisa dibuka?

<details>
<summary><b>▸ Jalan keliling kota</b> · Buka catatan level design</summary>

Saya membedah kota di *Blue Protocol*, *Monster Hunter*, dan *Final Fantasy*: bagaimana jalan mengarahkan pemain, di mana NPC masuk akal untuk ditemui, dan bagaimana props memberi petunjuk tentang fungsi suatu tempat. Itu referensi untuk iterasi berikutnya, bukan fitur yang sudah selesai di TOU.

</details>

<details>
<summary><b>▸ Masuk bengkel karakter</b> · Buka catatan sculpting</summary>

NPC sudah mulai dibuat, tapi hasil awalnya belum sesuai arah visual. Fokus saya sekarang adalah membenahi **siluet dan proporsi** dulu. Kalau bentuknya belum terbaca dari kamera third-person, menambah detail permukaan tidak akan menyelesaikan masalahnya.

</details>

<details>
<summary><b>▸ Ganti cartridge: LaMonth</b> · Eksperimen naratif</summary>

Di LaMonth, saya ingin pemain mengikuti cerita tanpa selalu diberi daftar quest. Tantangannya: bagaimana dialog dan kondisi tempat bisa membuat orang penasaran ke mana harus pergi, tanpa bikin mereka nyasar karena tidak ada petunjuk?

</details>

## 03 Systems Deck

### Lima proses. Satu kursi.

<details open>
<summary><b>▸ Buka hasil uji Reservasi Kursi</b> · Proyek kelompok</summary>

```text
SKENARIO : 5 proses memesan kursi yang sama
HASIL    : 1 berhasil, 4 ditolak
UJI      : 100/100 putaran lulus
```

Di proyek kelompok ini, kami memakai **C di Debian**. Status kursi disimpan di *shared memory*, dan semaphore menjaga supaya dua proses tidak membaca kursi yang sama sebagai “masih kosong” lalu sama-sama berhasil memesan.

</details>

<details>
<summary><b>▸ Buka terminal BMKG Earthquake Monitor</b> · Jenkins</summary>

Saya membuat job Jenkins terjadwal yang membaca data gempa BMKG, mencatat hasilnya, lalu mengirim notifikasi lewat **Telegram** dan **WhatsApp**. Satu kali jalan sukses di terminal belum cukup buat demo ini: saya juga perlu melihat job berjalan dari timer Jenkins.

</details>

## 04 Repo Vault

`A1` [Environment-GameDev](https://github.com/xenonnnn222/Environment-GameDev)  
`A2` [gamedev-mid-sam](https://github.com/xenonnnn222/gamedev-mid-sam)  
`B1` [PasarKu](https://github.com/xenonnnn222/PasarKu)

[▲ Kembali ke menu](#select-a-world)
