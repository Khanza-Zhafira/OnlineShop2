<script setup>
import ProductCard from '../components/ProductCard.vue'
const daftarProduk = [
  { id: 1, nama: 'Kucing Himalaya', harga: 15000000, gambar: 
'https://th.bing.com/th/id/OIP.JbwJo4291Ej2yj-bmfEzKAHaHG?w=234&h=180&c=7&r=0&o=7&pid=1.7&rm=3' },
  { id: 2, nama: 'Kucing Maine coon', harga: 7000000, gambar: 
'https://www.bing.com/th/id/OIP.LWNxEebk_9woafS2xGOydAHaE8?w=193&h=135&c=8&rs=1&qlt=90&o=6&pid=ImgAns&rm=2' },
  { id: 3, nama: 'Kucing Russian Blue', harga: 30000000, gambar: 
'https://www.bing.com/th/id/OIP.1fAz6KeCF_GOkAaU-REuIAHaD3?w=193&h=135&c=8&rs=1&qlt=90&o=6&pid=ImgAns&rm=2'},
]
</script>
<template>
  <main>
    <h1>Produk Kami</h1>
    <div class="grid">
      <ProductCard
        v-for="produk in daftarProduk"
        :key="produk.id"
        :nama="produk.nama"
        :harga="produk.harga"
        :gambar="produk.gambar"
      />
    </div>
  </main>
</template>
 
<style scoped>
.grid {
  display: flex;
  gap: 16px;
  flex-wrap: wrap;
}
</style>