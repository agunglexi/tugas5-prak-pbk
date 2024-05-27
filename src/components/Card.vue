<template>
    <div class="product-card">
      <div class="card">
        <div class="row no-gutters">
          <div class="col-md-4">
            <img class="card-img-top" :src="product.image" alt="Card image cap">
          </div>
          <div class="col-md-8">
            <div class="card-body">
              <h5 class="card-title">{{ product.name }}</h5>
              <p class="card-text">Price: ${{ product.price }}</p>
              <div class="btn-group">
                <button type="button" class="btn btn-sm btn-outline-secondary">View</button>
                <button type="button" class="btn btn-sm btn-outline-secondary">Add to Cart</button>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'Card',
    props: ['product']
  }
  </script>
  
  <style scoped>
  .product-card {
    margin-bottom: 30px; /* Jarak antara kartu produk */
  }
  
  .card {
    transition: transform 0.2s; /* Efek transisi ketika kartu digerakkan */
    width: 100%;
  }
  
  .card:hover {
    transform: translateY(-5px); /* Menggeser kartu ke atas ketika dihover */
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1); /* Bayangan kartu yang diubah saat dihover */
  }
  
  .card-img-top {
    height: 100px; /* Tinggi gambar kartu */
    object-fit: cover; /* Memastikan gambar kartu dipotong sesuai dengan ukuran yang ditentukan */
  }
  
  .card-title {
    font-size: 18px; /* Ukuran font judul kartu */
  }
  
  .card-text {
    font-size: 16px; /* Ukuran font teks kartu */
  }
  
  .btn-group {
    margin-top: 10px; /* Jarak antara grup tombol dan teks */
  }
  
  .btn {
    font-size: 14px; /* Ukuran font tombol */
    background-color: coral;
  }
  
  .btn-outline-secondary {
    color: white; /* Warna teks tombol */
    border-color: #6c757d; /* Warna border tombol */
  }
  
  .btn-outline-secondary:hover {
    background-color: #6c757d; /* Warna latar belakang tombol saat dihover */
    color: #fff; /* Warna teks tombol saat dihover */
  }
  </style>
  