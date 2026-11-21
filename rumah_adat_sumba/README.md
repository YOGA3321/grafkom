# Rumah Adat Sumba (Uma Mbatangu)

Model 3D rumah adat Sumba dengan atap menara tinggi, dibuat di Blender 5.2.

## Isi folder

| File | Isi |
|---|---|
| `rumah_adat_sumba_utuh.blend` | Scene lengkap: rumah, interior, 2 pohon, tanah, lampu, dan 5 kamera |
| `komponen/01_Atap_Jerami.blend` | Kulit atap jerami, susunan menara, rumbai, bubungan, tanduk puncak |
| `komponen/02_Rangka_Atap_Bambu.blend` | Kasau & reng bambu di bawah atap |
| `komponen/03_Pilar_Leli_Loteng.blend` | 4 pilar kayu, piringan *leli*, balok & lantai loteng |
| `komponen/04_Dinding_Bambu.blend` | Dinding bambu tegak + rangka kayu & kusen pintu |
| `komponen/05_Lantai_Panggung.blend` | Lantai bambu, tiang kolong, tangga & bangku beranda |
| `komponen/06_Meja_Bambu_L.blend` | Meja bambu bentuk L |
| `komponen/07_Perabot.blend` | Jerigen, termos, ember, piring, keranjang |
| `komponen/08_Bilik_Tidur.blend` | Dipan bambu, kasur tenun, bantal, dinding bilik, tirai |
| `komponen/09_Tungku_Tradisional.blend` | Tungku tiga batu, periuk, bara, kayu bakar, rak asap |
| `komponen/10_Pohon_Depan.blend` | Pohon di depan rumah |
| `komponen/11_Pohon_Belakang.blend` | Pohon di belakang rumah |
| `komponen/12_Tanah.blend` | Bidang tanah berumput |

Di file utuh, setiap komponen ada di collection dengan nama yang sama (`01_Atap_Jerami`, dst.),
ditambah `00_Kamera_Lampu`.

## Menggabungkan komponen

Setiap komponen menyimpan posisi aslinya, jadi kalau di-*append* ke file kosong, bagian-bagiannya
langsung pas tanpa perlu digeser:

1. Blender → **File › Append…**
2. Pilih file di `komponen/`, masuk ke folder **Collection**, lalu pilih collection-nya
   (atau masuk ke **Object** untuk mengambil satu objek saja).
3. Ulangi untuk komponen lain.

Material ikut terbawa. Material yang dipakai bersama (misalnya `Bambu_Tegak`) bisa muncul sebagai
`.001` kalau di-append dari beberapa file. Itu normal.

## Ukuran

- Bentang atap ±15,6 × 14,4 m, tinggi puncak ±13,5 m
- Lantai panggung 1 m di atas tanah
- Satuan: meter, sumbu Z ke atas, depan rumah menghadap −Y

`Atap.blend` di root repo adalah file atap terpisah yang sudah ada sebelumnya dan tidak diubah.
