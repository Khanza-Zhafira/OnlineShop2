<script setup>
import ProductCard from '../components/ProductCard.vue'

const daftarProduk = [
  {
    id: 1,
    nama: 'Kucing Himalaya',
    harga: 15000000,
    gambar:
      'https://th.bing.com/th/id/OIP.JbwJo4291Ej2yj-bmfEzKAHaHG?w=234&h=180&c=7&r=0&o=7&pid=1.7&rm=3',
  },
  {
    id: 2,
    nama: 'Kucing Maine Coon',
    harga: 7000000,
    gambar:
      'https://www.bing.com/th/id/OIP.LWNxEebk_9woafS2xGOydAHaE8?w=193&h=135&c=8&rs=1&qlt=90&o=6&pid=ImgAns&rm=2',
  },
  {
    id: 3,
    nama: 'Kucing Russian Blue',
    harga: 30000000,
    gambar:
      'https://www.bing.com/th/id/OIP.1fAz6KeCF_GOkAaU-REuIAHaD3?w=193&h=135&c=8&rs=1&qlt=90&o=6&pid=ImgAns&rm=2',
  },
]
</script>

<template>
  <main class="product-page">
    <section class="page-header">
      <p class="eyebrow">Collection</p>
      <h1>Produk Kami</h1>
    </section>

    <section class="grid">
      <ProductCard
        v-for="produk in daftarProduk"
        :key="produk.id"
        :nama="produk.nama"
        :harga="produk.harga"
        :gambar="produk.gambar"
      />
    </section>
  </main>
</template>

<style scoped>
.product-page {
  width: min(1200px, calc(100% - 32px));
  margin: 28px auto 56px;
}

.page-header {
  text-align: center;
  margin-bottom: 28px;
}

.eyebrow {
  margin: 0;
  font-size: 0.8rem;
  font-weight: 700;
  letter-spacing: 0.14em;
  text-transform: uppercase;
  color: #2d6cdf;
}

.page-header h1 {
  margin: 10px 0 0;
  font-size: clamp(2rem, 4vw, 2.8rem);
  color: #123a78;
}

.grid {
  display: grid;
  grid-template-columns: repeat(3, minmax(220px, 1fr));
  gap: 24px;
}

@media (max-width: 768px) {
  .grid {
    grid-template-columns: 1fr;
  }
}
</style>