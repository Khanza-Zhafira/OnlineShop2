<template>
  <main class="about-page">
    <section class="hero-box">
      <p class="eyebrow">About Us</p>
      <h1>Selamat Datang di Onlineshop Sekolah Kami</h1>
      <p>Belanja mudah, sekolah senang.</p>
      <button class="btn-grad">Click to Shop</button>
    </section>

    <section class="info-box">
      <h2>Tentang Kami</h2>
      <p>
        Onlineshop ini dikelola oleh siswa SMK Yadika Soreang jurusan RPL.
        Kami berkomitmen memberikan pengalaman belanja yang sederhana, aman,
        dan nyaman bagi seluruh siswa dan masyarakat sekitar.
      </p>
    </section>
  </main>
</template>

<style scoped>
.about-page {
  width: min(1200px, calc(100% - 32px));
  margin: 32px auto 48px;
  display: grid;
  gap: 24px;
}

.hero-box,
.info-box {
  background: linear-gradient(135deg, #edf5ff 0%, #ffffff 100%);
  border: 1px solid #e6edf9;
  border-radius: 26px;
  box-shadow: 0 16px 32px rgba(15, 23, 42, 0.06);
}

.hero-box {
  text-align: center;
  padding: 52px 28px;
  color: #123a78;
}

.eyebrow {
  margin: 0 0 10px;
  font-size: 0.8rem;
  font-weight: 700;
  letter-spacing: 0.14em;
  text-transform: uppercase;
  color: #2d6cdf;
}

.hero-box h1 {
  margin: 0;
  font-size: clamp(1.8rem, 4vw, 2.8rem);
}

.hero-box p {
  margin: 12px auto 0;
  max-width: 640px;
  color: #475569;
}

.btn-grad {
  margin-top: 24px;
  padding: 15px 32px;
  border: none;
  border-radius: 999px;
  background: linear-gradient(90deg, #2d6cdf 0%, #5fa8ff 100%);
  color: white;
  font-weight: 700;
  text-transform: uppercase;
  cursor: pointer;
  box-shadow: 0 12px 22px rgba(45, 108, 223, 0.2);
}

.info-box {
  padding: 32px 28px;
}

.info-box h2 {
  margin: 0 0 12px;
  color: #123a78;
  font-size: 2rem;
}

.info-box p {
  margin: 0;
  color: #475569;
  font-size: 1.02rem;
  line-height: 1.8;
}
</style>
