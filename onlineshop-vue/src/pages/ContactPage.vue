<template>
  <div class="contact-page">
    <section class="banner">
      <div class="banner-content">
        <p class="eyebrow">Contact</p>
        <h1>Hubungi Kami</h1>
      </div>
    </section>

    <section class="content">
      <div class="info-box">
        <h2>Info Kontak</h2>

        <div class="info-item">
          <h4>Alamat</h4>
          <p>Jl. Cipeer No. 1, Soreang, Kab. Bandung</p>
        </div>

        <div class="info-item">
          <h4>Telepon</h4>
          <p>(022) 123 4567</p>
        </div>

        <div class="info-item">
          <h4>Email</h4>
          <p>Info@smmkyadikasoreang.sch.id</p>
        </div>
      </div>

      <div class="form-box">
        <h2>Kirim Pesan</h2>

        <label>Nama</label>
        <input type="text" placeholder="Nama Kamu" />

        <label>Email</label>
        <input type="email" placeholder="Email Kamu" />

        <label>Pesan</label>
        <textarea placeholder="Tulis pesan kamu..."></textarea>

        <button>Kirim</button>
      </div>
    </section>

    <footer>
      SMK Yadika Soreang - Onlineshop Soreang
    </footer>
  </div>
</template>

<style scoped>
.contact-page {
  width: min(1200px, calc(100% - 32px));
  margin: 28px auto 50px;
  color: #1f2937;
}

.banner {
  background: linear-gradient(135deg, #2d6cdf 0%, #5ea5ff 100%);
  border-radius: 28px;
  box-shadow: 0 18px 36px rgba(45, 108, 223, 0.18);
  margin-bottom: 28px;
}

.banner-content {
  padding: 56px 20px;
  text-align: center;
  color: white;
}

.eyebrow {
  margin: 0 0 8px;
  font-size: 0.82rem;
  font-weight: 700;
  letter-spacing: 0.12em;
  text-transform: uppercase;
  opacity: 0.8;
}

.banner h1 {
  margin: 0;
  font-size: clamp(2rem, 4vw, 3rem);
}

.content {
  display: grid;
  grid-template-columns: 1fr 1.2fr;
  gap: 28px;
  align-items: start;
}

.info-box,
.form-box {
  background: rgba(255, 255, 255, 0.96);
  border: 1px solid #e6edf9;
  border-radius: 24px;
  padding: 30px 24px;
  box-shadow: 0 12px 28px rgba(15, 23, 42, 0.06);
}

.info-box h2,
.form-box h2 {
  margin: 0 0 22px;
  font-size: 1.7rem;
  color: #123a78;
}

.info-item {
  margin-bottom: 24px;
}

.info-item h4 {
  margin: 0 0 8px;
  font-size: 0.9rem;
  color: #2d6cdf;
  text-transform: uppercase;
  letter-spacing: 0.06em;
}

.info-item p {
  margin: 0;
  color: #475569;
  line-height: 1.7;
  font-size: 0.98rem;
}

.form-box {
  display: flex;
  flex-direction: column;
}

.form-box label {
  margin-bottom: 8px;
  font-size: 0.86rem;
  font-weight: 700;
  color: #334155;
}

.form-box input,
.form-box textarea {
  width: 100%;
  border: 1px solid #dbe5f3;
  border-radius: 12px;
  padding: 12px 14px;
  margin-bottom: 18px;
  font-size: 0.96rem;
  background: #f8fbff;
  transition: border-color 0.2s ease, box-shadow 0.2s ease;
}

.form-box input:focus,
.form-box textarea:focus {
  outline: none;
  border-color: #7aa9ff;
  box-shadow: 0 0 0 4px rgba(92, 138, 255, 0.12);
}

.form-box textarea {
  min-height: 110px;
  resize: vertical;
}

.form-box button {
  align-self: flex-start;
  border: none;
  border-radius: 999px;
  background: linear-gradient(90deg, #2d6cdf 0%, #5fa8ff 100%);
  color: white;
  font-weight: 700;
  padding: 12px 26px;
  cursor: pointer;
  box-shadow: 0 10px 20px rgba(45, 108, 223, 0.18);
}

footer {
  margin-top: 24px;
  text-align: center;
  padding-top: 20px;
  border-top: 1px solid #e2e8f0;
  color: #64748b;
  font-size: 0.9rem;
}

@media (max-width: 768px) {
  .content {
    grid-template-columns: 1fr;
  }
}
</style>