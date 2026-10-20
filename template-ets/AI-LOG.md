# AI-LOG

Catat setiap penggunaan AI yang menghasilkan kode. Jika tidak memakai AI sama sekali, tulis satu baris: **tidak memakai AI**.

Log yang jujur tidak mengurangi nilai, sebanyak apa pun AI dipakai. Yang mengurangi nilai adalah log yang tidak sesuai dengan kode, atau isi log yang tidak bisa dijelaskan.

## (Nama fitur atau fungsi, misalnya: Deteksi bentrok slot, B5)
- Prompt: (ringkas, apa yang kamu minta)
- Dipakai: (bagian kode yang kamu ambil, misalnya nama fungsi dan file)
- Diubah: (apa yang kamu ubah atau perbaiki dari hasil AI, dan kenapa)

## (Entri berikutnya)
- Prompt: kira2 bagaimana struktur objek/func sperti method ini punya siapa? apakah ada interface? dll
- Dipakai: -
- Diubah: 
- func (s *Store) GetSumberDaya(id int) (SumberDaya, bool) {
    // Cari sumber daya berdasarkan ID.
    // Implementasi menyusul.
    return SumberDaya{}, false
}

## (Entri berikutnya)
- Prompt: banyak kode yang di generate hasil autocomplete / inline suggestions
- Dipakai: store.go, api.go
- Diubah: store.go, api.go

## (Entri berikutnya)
- Prompt: cek 3 struct di store.go
- Dipakai: 3 struct di store.go
- Diubah: menambah Store utk masing2 struct

## (Entri berikutnya)
- Prompt: cek 3 store utk struct di store.go
- Dipakai: 3 store struct di store.go
- Diubah: mengubah 3 store menjadi satu store saja

## (Entri berikutnya)
- Prompt: filter opsional utk list peminjaman
- Dipakai: func (api *API) listPeminjaman, func (s *Store) ListPeminjaman.
- Diubah: mengaplikasikan filter