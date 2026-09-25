<template>
  <main class="landing-page">
    <section class="hero">
      <div class="hero-content">
        <p class="eyebrow">Onlineshop Athayy</p>
        <h1>Selamat Datang di Onlineshop Athayy</h1>
        <p class="subtitle">Belanja mudah, hati senang.</p>
        <button class="btn-grad">Click to Shop</button>
      </div>
    </section>

    <section class="features">
      <article class="feature-card">
        <div class="icon">💰</div>
        <h2>Harga Murah</h2>
        <p>Belanja mudah, hati senang.</p>
      </article>

      <article class="feature-card">
        <div class="icon">🩵</div>
        <h2>Pelayanan Terbaik</h2>
        <p>Melayani dengan sepenuh hati.</p>
      </article>

      <article class="feature-card">
        <div class="icon">✨</div>
        <h2>Produk Berkualitas</h2>
        <p>Produk yang kami jual berkualitas.</p>
      </article>
    </section>
  </main>
</template>

<style scoped>
.landing-page {
  width: 100%;
  min-height: 100vh;
  background: linear-gradient(180deg, #f5f9ff 0%, #eef5ff 100%);
}

.hero {
  width: min(1200px, calc(100% - 32px));
  margin: 0 auto;
  padding: 72px 0 36px;
}

.hero-content {
  background: linear-gradient(135deg, #2d6cdf 0%, #4ea0ff 100%);
  border-radius: 28px;
  padding: 72px 48px;
  text-align: center;
  color: #fff;
  box-shadow: 0 20px 45px rgba(45, 108, 223, 0.18);
}

.eyebrow {
  margin: 0 0 12px;
  font-size: 0.8rem;
  font-weight: 700;
  letter-spacing: 0.14em;
  text-transform: uppercase;
  opacity: 0.9;
}

.hero h1 {
  margin: 0;
  font-size: clamp(2rem, 4vw, 3.2rem);
  line-height: 1.2;
  font-weight: 800;
}

.subtitle {
  margin: 16px auto 0;
  font-size: 1.08rem;
  max-width: 640px;
  opacity: 0.95;
}

.btn-grad {
  margin-top: 28px;
  padding: 15px 32px;
  border: none;
  border-radius: 999px;
  background: linear-gradient(90deg, #ffffff 0%, #dfeeff 100%);
  color: #1f4da6;
  font-weight: 700;
  font-size: 0.92rem;
  letter-spacing: 0.04em;
  text-transform: uppercase;
  cursor: pointer;
  transition: transform 0.25s ease, box-shadow 0.25s ease;
  box-shadow: 0 12px 22px rgba(255, 255, 255, 0.2);
}

.btn-grad:hover {
  transform: translateY(-2px);
  box-shadow: 0 16px 28px rgba(255, 255, 255, 0.28);
}

.features {
  width: min(1200px, calc(100% - 32px));
  margin: 0 auto 56px;
  display: grid;
  grid-template-columns: repeat(3, minmax(220px, 1fr));
  gap: 24px;
}

.feature-card {
  background: rgba(255, 255, 255, 0.92);
  border: 1px solid #e6edf9;
  border-radius: 22px;
  padding: 32px 24px;
  text-align: center;
  box-shadow: 0 12px 28px rgba(15, 23, 42, 0.06);
}

.icon {
  width: 62px;
  height: 62px;
  margin: 0 auto 18px;
  display: grid;
  place-items: center;
  border-radius: 18px;
  background: linear-gradient(135deg, #dfeeff 0%, #eaf7ff 100%);
  font-size: 2rem;
}

.feature-card h2 {
  margin: 0 0 12px;
  font-size: 1.5rem;
  color: #123a78;
}

.feature-card p {
  margin: 0;
  color: var(--muted);
  font-size: 0.98rem;
  line-height: 1.7;
}

@media (max-width: 768px) {
  .hero-content {
    padding: 48px 22px;
  }

  .features {
    grid-template-columns: 1fr;
  }
}
</style>
