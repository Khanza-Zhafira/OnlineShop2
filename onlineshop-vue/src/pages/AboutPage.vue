<template>
<div class="landing-page">
    <h1 style="font-size: 20px;">SELAMAT DATANG DI ONLINESHOP SEKOLAH KAMI</h1>
    <P>Belanja mudah, seklah senang.</P>
    <button class="btn-grad">click to shop</button>
</div>

<main>
  <h1>Tentang Kami</h1>
  <p>Onlineshop ini di kelola oleh siswa SMK YADIKA SOREANG Jurusan RPL</p>
</main>
</template>
<style scoped>
.landing-page {
  flex-direction: column;
  justify-content: center;
  padding: 5rem;
  text-align: center;
  align-items: center;
  background-color: aquamarine;
  width: 100%;
  height: 100px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1)

}
.btn-grad {
  background-image: linear-gradient( to right, #77a1d3 0%, #79cbca 51%, #77a1d3 100%);
}

.btn-grad {
  margin: 10px;
  padding: 15px 45px;
  text-align: center;
  text-transform: uppercase;
  transition: 0.5s;
  background-size: 200% auto;
  color: white;
  box-shadow: 0 0 20px #eee;
  border-radius: 10px;
  outline: none;
  border: none;
}

.btn-grad:hover {
  background-position: right center;
  color: #fff;
  text-decoration: none;
}
</style>