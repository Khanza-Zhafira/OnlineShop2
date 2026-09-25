<script setup>
defineProps(['nama', 'harga', 'gambar'])
</script>

<template>
  <article class="card">
    <img :src="gambar" :alt="nama" />
    <div class="card-body">
      <h3>{{ nama }}</h3>
      <p>Rp {{ harga.toLocaleString('id-ID') }}</p>
      <button class="buy-btn">Beli</button>
    </div>
  </article>
</template>

<style scoped>
.card {
  background: rgba(255, 255, 255, 0.98);
  border: 1px solid #e6edf9;
  border-radius: 22px;
  overflow: hidden;
  box-shadow: 0 12px 28px rgba(15, 23, 42, 0.06);
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.card:hover {
  transform: translateY(-4px);
  box-shadow: 0 18px 32px rgba(15, 23, 42, 0.08);
}

.card img {
  width: 100%;
  height: 220px;
  object-fit: cover;
  display: block;
  background: #eaf3ff;
}

.card-body {
  padding: 18px 18px 20px;
}

.card h3 {
  margin: 0 0 10px;
  color: #123a78;
  font-size: 1.25rem;
}

.card p {
  margin: 0;
  color: #2d6cdf;
  font-weight: 700;
  font-size: 1rem;
}

.buy-btn {
  margin-top: 16px;
  width: 100%;
  border: none;
  border-radius: 12px;
  background: linear-gradient(90deg, #2d6cdf 0%, #5fa8ff 100%);
  color: white;
  font-weight: 700;
  padding: 12px 16px;
  cursor: pointer;
  transition: opacity 0.2s ease, transform 0.2s ease;
}

.buy-btn:hover {
  opacity: 0.95;
  transform: translateY(-1px);
}
</style>