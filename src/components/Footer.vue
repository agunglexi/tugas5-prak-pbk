<template>
    <footer class="footer mt-auto py-3 bg-light">
      <div class="container position-relative">
        <span class="text-muted position-absolute bottom-0 start-50 translate-middle-x">©Hak Cipta 2024 Lexsi Automotif</span>
      </div>
    </footer>
  </template>
  
  <script>
  export default {
    name: 'Footer'
  }
  </script>
  
  <style scoped>
  .footer {
    /* Mengatur footer tetap di bagian bawah halaman */
    background-color: rgb(211, 210, 210);
    width: 100%;
    color: #6c757d; /* Warna teks footer */
    text-align: center; /* Pusatkan teks footer */
    padding: 10px 0; /* Padding atas dan bawah footer */
    position: absolute;
  }
  
  .footer:hover {
    background-color: #e9ecef; /* Warna latar belakang footer saat dihover */
    width: 100%
  }
  
  /* Stil teks */
  .text-muted {
    font-size: 14px; /* Ukuran font teks */
    width: 100%
  }
  </style>
  