<template>
    <div class="contact-page">

        <section class="banner">
            <h1>Hubungi Kami</h1>
        </section>

        <section class="content">

            <div class="Info">
                <h2>Info Kontak</h2>

                <div class="info-item">
                    <h4>Alamat</h4>
                    <p>Jl. Cipeer No. 1, Soreang, Kab.Bandung</p>
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


            <div class="form">
                <h2>Kirim Pesan</h2>

                <label>Nama</label>
                <input type="text" placeholder="Nama Kamu">

                <label>Email</label>
                <input type="email" placeholder="Email Kamu">

                <label>Pesan</label>
                <textrea placeholder="Tulis pesan kamu..."></textrea>

                <button>Kirim</button>
            </div>
        </section>
        <footer>
            SMK Yadika Soreang - Onlineshop Soreang
        </footer>
    </div>
</template>

<style scoped>
* {
    box-sizing: border-box;
}

.contact-page {
    font-family: arial, sans-serif;
    color: skyblue;
    min-height: 100vh;
}

.navbar {
    width: 70%;
    margin: auto;
    height: 70px;

    display: flex;
    align-items: center;
    justify-content: space-between;
}

.menu {
    display: flex;
    gap: 25;
}

.menu a {
    text-decoration: none;
    color: #333;
    font-size: 13px;
}

.menu .active {
    color: #2878bd;
    border-bottom: 2px solid #2878bd;
    padding-bottom: 5px;
}
</style>