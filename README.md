# qa-sdlc-simulasi
SDLC (Software Development Life Cycle) adalah proses terstruktur yang digunakan untuk merancang, mengembangkan, menguji, dan memelihara perangkat lunak.

# QA Engineer Simulation Project

##  Tujuan
Repositori ini dibuat untuk mensimulasikan peran QA Engineer dalam proses pengujian aplikasi berbasis client-server. Fokus utama adalah memahami alur data dari database ke API, lalu ke client, serta bagaimana QA menguji dan memvalidasi setiap tahap.

##  Konsep yang Diuji
- Client-Server Architecture
- API Testing (GET, POST)
- JSON Parsing & Validation
- SQL & Data Integrity
- Cookies & Cache Behavior

##  Tools yang Digunakan
- Postman
- Python (requests, json)
- VS Code
- GitHub

##  Struktur Folder

## qa-sdlc-simulasi
├── README.md (Penjelasan alur simulasi SDLC)
├── requirements/
│   └── user-stories.md
├── test-cases/
│   └── TC001_lihat_produk.md
├── bug-reports/
│   └── BR001_stok_negatif.md
├── postman/
│   └── api_tests_collection.json
└── assets/
    └── diagram-client-server.png

    
##  Dummy API
Simulasi API menggunakan file JSON sebagai response. Cocok untuk latihan testing API dan validasi data.

##  Peran QA
QA bertanggung jawab untuk:
- Menyusun test case berdasarkan kebutuhan
- Melakukan pengujian API dan UI
- Validasi data JSON terhadap database
- Dokumentasi bug dan hasil pengujian

##  Catatan
Dokumentasi ini adalah bagian dari portofolio pembelajaran saya sebagai QA Engineer. Tujuannya adalah menunjukkan pemahaman teknis dan kemampuan analisis dalam proses pengujian perangkat lunak.

# TC001 - Lihat Produk

## Tujuan
Memastikan bahwa detail produk ditampilkan dengan benar saat pengguna mengakses endpoint `/produk/1`.

## Prasyarat
- Data produk tersedia di database
- API endpoint aktif

## Langkah Pengujian
1. Kirim request `GET /produk/1` via Postman
2. Periksa response JSON
3. Validasi field: `nama`, `harga`, `stok`

## Data Uji
```json
{
  "id": 1,
  "nama": "Headphone Bluetooth",
  "harga": 299000,
  "stok": 25
}
```

Hasil yang Diharapkan
Status code: 200 OK

Semua field muncul dan sesuai

Hasil Aktual
Sesuai dengan ekspektasi

Status
PASS


---

