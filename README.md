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

## 3. Selector dalam CSS
Selector digunakan untuk memilih elemen yang akan diberikan gaya.

### a. Selector Dasar
- **Selector Elemen**: Memilih elemen berdasarkan tag.
  ```css
  p {
    color: green;
  }
  ```
- **Selector ID**: Memilih elemen berdasarkan atribut `id`.
  ```css
  #judul {
    font-size: 24px;
  }
  ```
- **Selector Class**: Memilih elemen berdasarkan atribut `class`.
  ```css
  .highlight {
    background-color: yellow;
  }
  ```

### b. Selector Lanjutan
- **Selector Child (`>`)**: Memilih elemen yang merupakan anak langsung dari elemen tertentu.
  ```css
  div > p {
    color: blue;
  }
  ```
- **Selector Descendant (spasi)**: Memilih elemen di dalam elemen lain tanpa memperhatikan tingkat kedalaman.
  ```css
  div p {
    font-style: italic;
  }
  ```
- **Selector Adjacent Sibling (`+`)**: Memilih elemen yang langsung mengikuti elemen tertentu.
  ```css
  h1 + p {
    font-weight: bold;
  }
  ```

## 4. Properti CSS Dasar

### a. Warna dan Latar Belakang
- `color`: Mengubah warna teks.
- `background-color`: Mengubah warna latar belakang.
  ```css
  body {
    background-color: lightgray;
  }
  ```

### b. Teks dan Font
- `font-family`: Mengatur jenis font.
- `font-size`: Mengatur ukuran font.
- `text-align`: Mengatur perataan teks (left, center, right, justify).
  ```css
  h1 {
    font-family: Arial, sans-serif;
    text-align: center;
  }
  ```

### c. Ukuran dan Jarak
- `width` dan `height`: Mengatur lebar dan tinggi elemen.
- `margin`: Mengatur jarak luar elemen.
- `padding`: Mengatur jarak dalam elemen.
  ```css
  div {
    width: 300px;
    height: 200px;
    margin: 20px;
    padding: 10px;
  }
  ```

## 5. Layout dengan CSS
### a. Display
- `block`: Elemen menempati satu baris penuh.
- `inline`: Elemen hanya selebar kontennya.
- `flex`: Mengatur elemen secara fleksibel.
  ```css
  .container {
    display: flex;
    justify-content: center;
  }
  ```

### b. Position
- `static` (default)
- `relative`
- `absolute`
- `fixed`
  ```css
  .box {
    position: absolute;
    top: 50px;
    left: 100px;
  }
  ```

## 6. Responsif dengan CSS
### a. Media Query
Digunakan untuk membuat tampilan yang responsif di berbagai ukuran layar.
```css
@media (max-width: 600px) {
  body {
    background-color: lightblue;
  }
}
```

### b. Flexbox dan Grid
- **Flexbox** digunakan untuk tata letak yang fleksibel.
  ```css
  .container {
    display: flex;
    justify-content: space-between;
  }
  ```
- **CSS Grid** digunakan untuk tata letak berbasis grid.
  ```css
  .grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
  }
  ```

## 7. Animasi dan Transisi
- `transition`: Efek perubahan yang halus.
  ```css
  button {
    transition: background-color 0.3s;
  }
  ```
- `animation`: Membuat animasi kustom.
  ```css
  @keyframes example {
    from {background-color: red;}
    to {background-color: yellow;}
  }
  div {
    animation: example 2s infinite;
  }
  ```

## 8. Kesimpulan
CSS memungkinkan kita untuk mengatur tampilan halaman web dengan fleksibel. Dengan memahami dasar-dasar CSS seperti selector, properti, layout, dan animasi, kita dapat menciptakan desain web yang menarik dan responsif.
