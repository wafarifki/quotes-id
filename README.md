# Taskbar Clock Customization (Windhawk)

Konfigurasi **Taskbar Clock Customization** untuk **Windhawk** dengan tampilan **minimalis & modern**, menampilkan **CPU & RAM**, serta **tooltip berisi quote motivasi Bahasa Indonesia** yang **auto rotate** dari sumber eksternal.
Cocok untuk **developer**, **power user**, dan siapa pun yang ingin taskbar lebih informatif tapi tetap bersih.

---

## Fitur Utama

- Format jam & tanggal ringkas
- Informasi performa real-time (CPU & RAM)
- Tooltip **custom (replace tooltip Windows)**
- Quote motivasi **Bahasa Indonesia**
- **Auto rotate quote** tanpa script tambahan
- Menggunakan font bawaan Windows 11
- Stabil & ringan

---

## Tentang Repositori `quotes-id`

### Apa itu `quotes-id`?
`quotes-id` adalah repositori **JSON** yang berisi kumpulan **quote singkat Bahasa Indonesia**.

### Fungsinya
- Menjadi **sumber quote** untuk tooltip
- Quote bisa di-update kapan saja tanpa mengubah konfigurasi Windhawk
- Membuat tooltip terasa hidup karena konten **berubah otomatis**
---

## Tutorial Instalasi Windhawk
1. Buka situs resmi Windhawk  
   https://windhawk.net atau download melalui link berikut: https://ramensoftware.com/downloads/windhawk_setup.exe
3. Download versi terbaru
4. Jalankan installer
5. Selesaikan proses instalasi

Setelah terpasang, Windhawk akan berjalan di background Windows.

---

## **Tutorial Instalasi Mod Taskbar Clock Customization**

1. Buka aplikasi **Windhawk**
2. Masuk ke tab **Explore / Jelajahi**
3. Cari / ketikkan kata kunci **Taskbar Clock Customization**
4. Klik **Install / Pasang**
5. Tunggu hingga statusnya menjadi **Installed / Terpasang**

---

## Tutorial Menerapkan Konfigurasi Mod Taskbar Clock Customization

### 1. Buka Pengaturan Mod
1.1. Klik **Details / Rincian** di Taskbar Clock Customization  
1.2. Klik tab **Settings / Pengaturan**  
1.3. Klik **Textual Mode**

### 2. Paste Konfigurasi Berikut
2.1 Salin dan tempel **seluruh konfigurasi** di bawah ini:

```yaml
ShowSeconds: 0
TimeFormat: HH':'mm
DateFormat: dd MMM yyyy
WeekdayFormat: ddd

TopLine: '%weekday%, %date% | %time%'
BottomLine: CPU %cpu% | RAM %ram%

TooltipLine: '%weekday%, %date% | %time%%n%%web1_full%'
TooltipLineMode: replace

Width: 120
Height: 48
MaxWidth: 0
TextSpacing: 0

WebContentsItems:
  - Url: https://quotes-id-random.wafarifqianafin.workers.dev/
    BlockStart: ''
    Start: ''
    End: ''
    ContentMode: xmlHtml
    SearchReplace:
      - Search: ''
        Replace: ''
    MaxLength: 80
WebContentsUpdateInterval: 10

TimeZones:
  - Asia/Jakarta

TimeStyle:
  Hidden: 0
  TextColor: '#F3F4F6'
  TextAlignment: center
  FontSize: 12
  FontFamily: Segoe UI Variable
  FontWeight: semibold
  FontStyle: normal
  FontStretch: normal
  CharacterSpacing: 0

DateStyle:
  Hidden: 0
  TextColor: '#9CA3AF'
  TextAlignment: center
  FontSize: 11
  FontFamily: Segoe UI Variable
  FontWeight: normal
  FontStyle: normal
  FontStretch: normal
  CharacterSpacing: 0
  
oldTaskbarOnWin11: 0
```

### 3. Simpan & Aktifkan
3.1. Klik **Save / Simpan pengaturan**  
3.2. Tunggu Explorer restart otomatis beberapa detik  
3.3. Selesai

---

## ✨ Contoh Hasil

Berikut tampilan akhir **Taskbar Clock Customization** setelah konfigurasi diterapkan.

### Tampilan Taskbar (Normal)

Menampilkan informasi waktu, tanggal, serta penggunaan CPU dan RAM secara ringkas dan bersih.

<p align="center">
  <img width="440" height="60" alt="Tampilan Taskbar" src="https://github.com/user-attachments/assets/319304f6-bfa9-4a82-975b-7e1652acdf18" />
</p>



### Tampilan Tooltip (Saat Di-hover)

Saat kursor diarahkan ke jam, tooltip akan menampilkan:
- Waktu & tanggal
- Quote motivasi Bahasa Indonesia
- Quote berubah otomatis (auto rotate)

<p align="center">
  <img width="450" height="168" alt="Tampilan Tooltip" src="https://github.com/user-attachments/assets/fb94da72-40bb-4ec9-8908-a66136067bca" />
</p>


> 💡 **Catatan:**  
> Quote di tooltip akan berganti secara otomatis setiap beberapa detik sesuai dengan konfigurasi `WebContentsUpdateInterval`.
