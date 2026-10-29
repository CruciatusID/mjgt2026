# 05 — SPESIFIKASI DAN PROMPT EKSPANSI OUTPAINT 16:9

## Geometri & Prinsip Penguncian
- **Rasio Kanvas Asal:** 4:3 (misal: 1536 × 1152 piksel).
- **Rasio Kanvas Target:** 16:9 (misal: 2048 × 1152 piksel pada tinggi yang sama).
- **Penempatan Master:** 4:3 master dikunci tepat di **75% lebar sentral** (tengah kanvas).
- **Sayap Ekstensibilitas (Outpaint Wings):** Masing-masing 12.5% di sayap kiri (+256 px) dan 12.5% di sayap kanan (+256 px).
- **Integritas Piksel:** Area master 4:3 tengah tidak boleh dipotong, di-zoom, digeser, atau diubah pencahayaannya. Seluruh elemen cerita, figur Paulus, pemuda, dan ruang negatif judul tetap 100% berada di 4:3 sentral.

---

## Konten Ekstensi Sayap
- **Sayap Kiri (12.5% lebar):** Kelanjutan dinding batu bata tanah liat kuno yang temaram, gantungan pasak kayu sederhana dengan beberapa helai tali rami kering, serta sebuah kendi tembikar tanah liat kecil di sudut lantai bersahaja.
- **Sayap Kanan (12.5% lebar):** Kelanjutan rak kayu bengkel dengan tumpukan gulungan kain tenun kasar, serta tepi kusen pintu kayu tua yang memperlihatkan secuil langit malam Mediterania yang gelap dan tenang dengan sedikit taburan bintang redup di kejauhan.
- **Larangan Keras:** Dilarang menambahkan figur manusia baru, dilarang menambahkan teks, simbol religius melayang, atau objek dramatis yang mengalihkan perhatian dari subjek utama di tengah.

---

## Outpainting Prompt (Untuk Inpainting / Generative Expand Tool)

```text
Symmetric horizontal canvas expansion of the approved 4:3 master painting to 16:9 widescreen format, seamlessly extending only the left and right background margins while keeping the central 75% master artwork completely locked and untouched.

Extend the rustic 1st-century workshop interior naturally:
On the left wing: Continue the ancient earthen mud-brick wall texture, soft chiaroscuro umber shadows, simple wooden wall pegs holding hanging coils of natural hemp twine, and a weathered small terracotta water jug resting on the packed dirt floor in the corner.
On the right wing: Continue the wooden workshop shelving holding extra rolls of dark woven goat-hair canvas, and the subtle vertical beam of an aged wooden doorway framing a glimpse of the quiet dark blue night sky outside with a few faint distant stars.

Maintain identical painterly 3D visual DNA: palpable, expressive impasto and gouache brushstrokes, matte non-glossy material textures, consistent lighting temperature from the central oil lamp, and matching atmospheric depth. Perfectly seamless blends at the borders with no seams, no repeats, no new human figures, no text, and no competing narrative objects.
```

---

## Validasi Crop-Back Check
Potongan 75% tengah dari hasil akhir 16:9 harus menghasilkan kembali komposisi master 4:3 asli secara sempurna tanpa distorsi anatomi, pergeseran horizon, atau kehilangan ruang negatif judul.
*Catatan Kejujuran Teknis:* Jika software image generation tidak mendukung *pixel-locking mask* dan melakukan *resynthesis*, lakukan audit visual diferensial ketat (zero lost details, tidak ada pergeseran wajah atau tangan) dan laporkan statusnya secara transparan.

