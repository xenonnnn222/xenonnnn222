![Marcellyno · Developer Cartridge](./pixel-banner.svg)

![Player 01 · Marcellyno · Informatika](./pixel-ui/hud.png)

> Di Unity, saya bisa bikin kota yang enak dilihat tapi masih terasa kosong. Di WhatsApp, saya bisa bikin agent yang jawabannya meyakinkan tapi belum tentu mencatat pesanan yang benar. Saya suka bagian setelah prototipe pertama jadi: mencari tahu **apa yang masih gagal**, lalu memperbaikinya.

<a name="select-a-world"></a>

## ![Select a world](./pixel-ui/start.png)
<p align="center">
  <a href="#01-ai-lab"><img src="./pixel-ui/menu-01.png" alt="01 · AI LAB" width="47%"></a>
  <a href="#02-game-studio"><img src="./pixel-ui/menu-02.png" alt="02 · GAME STUDIO" width="47%"></a>
</p>
<p align="center">
  <a href="#03-systems-deck"><img src="./pixel-ui/menu-03.png" alt="03 · SYSTEMS DECK" width="47%"></a>
  <a href="#04-repo-vault"><img src="./pixel-ui/menu-04.png" alt="04 · REPO VAULT" width="47%"></a>
</p>

<a name="01-ai-lab"></a>

## ![01 · AI LAB](./pixel-ui/world-01.png)

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

<a name="02-game-studio"></a>

## ![02 · GAME STUDIO](./pixel-ui/world-02.png)

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

<a name="03-systems-deck"></a>

## ![03 · SYSTEMS DECK](./pixel-ui/world-03.png)

### Fish Tea

Salah satu proyek game saya di **Roblox**.

<details>
<summary><b>▸ Buka terminal BMKG Earthquake Monitor</b> · Jenkins</summary>

Saya membuat job Jenkins terjadwal yang membaca data gempa BMKG, mencatat hasilnya, lalu mengirim notifikasi lewat **Telegram** dan **WhatsApp**. Satu kali jalan sukses di terminal belum cukup buat demo ini: saya juga perlu melihat job berjalan dari timer Jenkins.

</details>

<a name="04-repo-vault"></a>

## ![04 · REPO VAULT](./pixel-ui/world-04.png)

`A1` [Environment-GameDev](https://github.com/xenonnnn222/Environment-GameDev)  
`A2` [gamedev-mid-sam](https://github.com/xenonnnn222/gamedev-mid-sam)  
`B1` [PasarKu](https://github.com/xenonnnn222/PasarKu)

[![Kembali ke menu Select a World](./pixel-ui/end.png)](#select-a-world)
