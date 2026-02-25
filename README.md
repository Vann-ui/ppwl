# PPWL3 - Praktikum Tailwind CSS 
  
## PRAKTIKUM 2: Perbedaan Tailwind v3 & v4 
  
**2 Perbedaan Utama Tailwind v3 & v4:** 
  
1. Konfigurasi:  
   - v3: Menggunakan tailwind.config.js  
   - v4: Menggunakan @theme directive di CSS 
  
2. Engine/Performa:  
   - v3: PostCSS-based processing  
   - v4: Oxide engine (Rust-based) - lebih cepat 
  
---  
  
## 1.3 Perbedaan Dengan Framework Tradisional Seperti Bootstrap 
  
### Bootstrap - Component-Based Framework  
Bootstrap menyediakan komponen siap pakai: 
<button class="btn btn-primary">Simpan</button> 
  
### Tailwind CSS - Utility-First Framework  
Tailwind memberikan utility classes untuk styling: 
<button class="bg-blue-500 text-white px-4 py-2 rounded">Simpan</button> 
  
### Perbedaan Utama: 
| Aspek | Bootstrap | Tailwind CSS | 
|-------|-----------|--------------| 
| Pendekatan | Component-based | Utility-first | 
| Ukuran File | Lebih besar | Lebih kecil | 
| Kustomisasi | Override CSS | Utility classes | 
| Fleksibilitas | Terbatas | Sangat fleksibel | 
| Learning Curve | Mudah | Perlu belajar utility | 
  
---  
  
## PRAKTIKUM 4: Box Model Answer 
  
**Pertanyaan:** Jika memberi warna pada latar belakang elemen, cth. bg-blue-600, maka Komponen box model yang terpengaruh warna latar adalah? 
  
**Jawaban:**  
Ketika menggunakan bg-blue-600 (background color), komponen Box Model yang terpengaruh warna latar adalah: 
  
1. **Content** - Isi elemen (text, gambar) akan memiliki latar belakang berwarna  
2. **Padding** - Area padding di dalam elemen juga terisi warna latar  
3. **Border** - Area border juga terpengaruh jika background-color di-apply 
  
**Yang TIDAK terpengaruh:**  
- **Outline** - Garis di luar border, tidak menempati ruang  
- **Margin** - Jarak luar elemen, transparan 
  
---  
  
## PRAKTIKUM 5: Flexbox  
File: flex.html  
- Menggunakan Flexbox untuk layout  
- Responsive: flex-col di mobile, flex-row di desktop (md:) 
  
---  
  
## PRAKTIKUM 6: Grid Responsive  
File: grid.html  
- Grid layout dengan 3 item child (warna berbeda: red, green, blue)  
- Responsive: grid-cols-1 di mobile, grid-cols-3 di desktop  
- Parent height: h-screen (viewport height)  
- Direction: Y (column) di mobile, X (row) di desktop 
  
---  
  
## PRAKTIKUM 7: Dark Mode  
File: dark.html  
- Button dengan dark mode class: dark:bg-red-100 dark:text-gray-800  
- Parent element: bg-sky-900 h-screen  
- Toggle manual menggunakan JavaScript (addClass/removeClass 'dark')  
- Tailwind config: darkMode: 'class' 
  
---  
  
## PRAKTIKUM 8: Custom Component dengan @apply  
File: custom.html  
- Custom class dibuat di @layer components  
- Menggunakan @apply directive untuk membungkus utility classes  
  
**Custom classes yang dibuat:**  
- .tab-button: px-4 py-2 text-sm font-medium border-b-2 transition  
- .tab-button-active: border-blue-500 text-blue-600  
- .tab-button-inactive: border-transparent text-gray-500 hover:text-blue-600 hover:border-blue-300 
  
---  
  
## Daftar File HTML  
| File | Deskripsi |  
|-----|-------------|  
| index.html | Hello World dengan Tailwind |  
| bs.html | Bootstrap Component Example |  
| tw.html | Tailwind Utility Example |  
| flex.html | Flexbox Layout |  
| grid.html | Grid Responsive Layout |  
| dark.html | Dark Mode Toggle |  
| custom.html | Custom Component dengan @apply | 
