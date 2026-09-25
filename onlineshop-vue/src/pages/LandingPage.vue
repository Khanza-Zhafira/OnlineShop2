<template>
 <main>

<div class="judul">
 <h1>Selamat Datang di Onlineshop Athayy</h1>
 <p>Belanja mudah, Hati Senang</p>
 <button class="btn-grad">Click to Shop</button>
</div>
 
<div class="container">

  <div class="landing-page1">
    <b>💰</b>
    <h1>harga murah</h1>
    <p>Belanja mudah, Hati senang</p>
  </div>
  
  <div class="landing-page1">
    <b>🩵</b>
    <h1>pelayanan terbaik</h1>
    <p>melayani dengan sepenuh hati.</p>
  </div>
  
  <div class="landing-page2">
    <b>✨</b>
    <h1>Produk Berkualitas</h1>
    <p>Produk yang kami jual Berkualitas</p>
  </div>
</div>

 </main>
 </template> 

 <style scoped> 
        .judul {
          witdh: 100%;
          height: 200px;
          background-color: #5798e2;
          text-align:center;
          padding-top: 2rem;
          color: white;
        }
        
        .container {
          display: flex;
          gap: 10px;
          justify-content: center;
          margin-top: 10px;
        }
        .landingPage1 {
          background-color: skyblue;
          height: 10rem;
          width: 20rem;
          border-radius: 10px;
          text-align: center;
          padding-top: 40px;
          color:bisque;          
        }
        
        .btm-grad {
        background-image: linear-gradient(to right, #77a1d3 0%, #79cbca 51%, #77a1d3 100%);        
        }
        .btn-grad {
          margin: 10px;
          padding: 15px 45px;
          text-align: center;
          text-transform: uppercase;
          transition: 0,5s;
          background-size: 200% auto;
          color:antiquewhite;
          box-shadow: 0 0 20px #eee;
          border-radius: 10px;
          outline: none;
          border: none;
        }
        
        .btn-grad:hover {
          background-position: right center;
          color: #fff;
          text-decoration: none;         
        }</style>