# API Harga Emas Indonesia

API ini menyediakan data harga emas dari berbagai brand di Indonesia, termasuk:

- **GALERI 24**
- **DINAR G24**
- **BABY GALERI 24**
- **ANTAM**
- **UBS**
- **ANTAM MULIA RETRO**
- **ANTAM NON PEGADAIAN**
- **LOTUS ARCHI**
- **UBS DISNEY**
- **UBS ELSA**
- **UBS ANNA**
- **UBS MICKEY FULLBODY**
- **LOTUS ARCHI GIFT**
- **UBS HELLO KITTY**
- **BABY SERIES TUMBUHAN**
- **BABY SERIES INVESTASI**
- **BATIK SERIES**

Data diperbarui **setiap 6 jam**, diambil langsung dari website [Galeri 24](https://galeri24.co.id/).

## 🚀 Cara Penggunaan

### **1. Mendapatkan Semua Harga Emas**

**Endpoint:**

```http
GET https://emas.maulanar.my.id/api/prices
```

**Contoh Response:**

```json
[
  {
    "brand": "GALERI 24",
    "weight": 0.5,
    "sell_price": 891000,
    "buyback_price": 770000,
    "updated_at": "2025-02-17"
  },
  ...
]
```

### **Penjelasan Response:**

- **`brand`** → Nama brand emas.
- **`weight`** → Berat emas dalam gram.
- **`sell_price`** → Harga jual emas dalam Rupiah (IDR).
- **`buyback_price`** → Harga buyback (jual kembali) dalam Rupiah (IDR).
- **`updated_at`** → Waktu pembaruan data dalam format Y-m-d.

---

### D\*\* Mendapatkan Harga Emas Berdasarkan Brand\*\*

**Endpoint:**

```http
GET https://emas.maulanar.my.id/api/prices/{brand}
```

**Contoh:** Untuk mendapatkan harga emas merek "ANTAM":

```http
GET https://emas.maulanar.my.id/api/prices/ANTAM
```

**Contoh:** Untuk mendapatkan harga emas merek "ANTAM" Berdasarkan Tanggal (COMING SOON):

```http
???
```

---

## 🎯 Manfaat API Ini

- Mendapatkan informasi harga emas dari berbagai brand dengan mudah.
- Data selalu diperbarui otomatis setiap **6 jam**.
- Dapat digunakan untuk aplikasi investasi emas atau e-commerce.

✨ **Semoga bermanfaat!** ✨asd
