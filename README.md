# Belajar CSS

## 1. Pendahuluan CSS
CSS (Cascading Style Sheets) adalah bahasa yang digunakan untuk mengatur tampilan elemen HTML. Dengan CSS, kita dapat mengontrol warna, ukuran, tata letak, dan berbagai aspek visual lainnya dari halaman web.

## 2. Cara Menggunakan CSS
Ada tiga cara untuk menerapkan CSS pada HTML:
- **Inline CSS**: Menulis CSS langsung dalam elemen HTML menggunakan atribut `style`.
  ```html
  <p style="color: red; font-size: 16px;">Teks berwarna merah</p>
  ```
- **Internal CSS**: Menulis CSS di dalam tag `<style>` dalam file HTML.
  ```html
  <style>
    p {
      color: blue;
      font-size: 18px;
    }
  </style>
  ```
- **External CSS**: Menulis CSS dalam file terpisah (`.css`) dan menghubungkannya dengan HTML menggunakan `<link>`.
  ```html
  <link rel="stylesheet" href="styles.css">
  ```
