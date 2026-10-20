# PROSES

## 1. Persona dan masalahnya
Dalam Persona E, yang menjadi pengguna adalah Asisten Lab yang bisa mengatur jadwal penggunaan atau peminjaman lab. masalahnya terkadang lab mempunyai jadwal tertentu dimana lab tersebut tidak bisa dipakai, pada situasi tersebut aslab bisa menutup jadwal peminjaman dan memblokir jadwal yang sudah terlanjur di-booking.

## 2. Rancangan struktur data
(Tulis struct dan slice/map apa yang kamu simpan, dan kenapa dipilih begitu. Rancang ini sebelum menulis kode, lalu catat kalau berubah di tengah jalan.)

di requirement ada beberapa fitur konkret yang diminta, `SumberDaya` dan `Peminjaman` dari fitur umum, dan `Blokir` dari fitur khusus Persona E.

```
// fitur umum
type SumberDaya struct {
    ID    int    `json:"id"`
    Nama  string `json:"nama"`
    Jenis string `json:"jenis"`
    Stok  int    `json:"stok"`
}

type Peminjaman struct {
    ID            int    `json:"id"`
    SumberDayaID  int    `json:"sumber_daya_id"`
    Peminjam      string `json:"peminjam"`
    Tanggal       string `json:"tanggal"`
    SlotMulai     int    `json:"slot_mulai"`
    SlotSelesai   int    `json:"slot_selesai"`
    Jumlah        int    `json:"jumlah"`
    Status        string `json:"status"`
}

// fitur khusus
type Blokir struct {
    ID           int    `json:"id"`
    SumberDayaID int    `json:"sumber_daya_id"`
    Tanggal      string `json:"tanggal"`
    SlotMulai    int    `json:"slot_mulai"`
    SlotSelesai  int    `json:"slot_selesai"`
    Keterangan   string `json:"keterangan"`
}

```
## 3. Satu keputusan desain
(Satu keputusan yang kamu ambil, pilihan lain yang kamu pertimbangkan, dan alasanmu memilih yang ini. Contoh: kenapa cek bentrok per slot, bukan per rentang.)

## 4. Bug atau kendala (minimal dua)
### Bug 1
- Gejala:
- Cara menemukan:
- Penyebab dan solusi:

### Bug 2
- Gejala:
- Cara menemukan:
- Penyebab dan solusi:

## 5. Change request
(Apa yang diminta, bagian kode mana yang kamu ubah, dan satu keputusan desain yang kamu ambil.)
