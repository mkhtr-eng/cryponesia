# cryponesia
website cryptocurrency
<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>CryptoNesia - Komunitas Crypto Indonesia</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css"/>
  <style>
    :root {
      --bg: #0a0a0f;
      --card: #12121a;
      --border: #1e1e2e;
      --accent: #00ff9d;
      --text: #ffffff;
      --muted: #aaaaaa;
    }
    * { margin:0; padding:0; box-sizing:border-box; }
    body { background:var(--bg); color:var(--text); font-family:'Inter', 'Segoe UI', sans-serif; min-height:100vh; }
    .container { max-width:1200px; margin:0 auto; padding:0 20px; }

    /* Header */
    header {
      background:linear-gradient(135deg, #11111a, #0a0a0f);
      padding:5rem 0 4rem;
      text-align:center;
      position:relative;
      overflow:hidden;
    }
    header::before {
      content:''; position:absolute; top:0; left:0; right:0; bottom:0;
      background:radial-gradient(circle at center, rgba(0,255,157,0.1), transparent 70%);
    }
    h1 {
      font-size:3.2rem;
      background:linear-gradient(90deg, #00ff9d, #00d4ff);
      -webkit-background-clip:text;
      -webkit-text-fill-color:transparent;
      margin-bottom:0.5rem;
      position:relative;
    }
    .subtitle { font-size:1.4rem; color:var(--muted); margin-top:1rem; }

    /* Features */
    .features {
      display:grid;
      grid-template-columns:repeat(auto-fit, minmax(300px,1fr));
      gap:2rem;
      padding:4rem 0;
    }
    .card {
      background:var(--card);
      border:1px solid var(--border);
      padding:2rem;
      border-radius:20px;
      transition:0.4s;
      text-align:center;
    }
    .card:hover {
      transform:translateY(-12px);
      border-color:var(--accent);
      box-shadow:0 20px 40px rgba(0,255,157,0.15);
    }
    .card i { font-size:3.5rem; color:var(--accent); margin-bottom:1rem; }

    /* Form Join Member */
    .join-section {
      background:var(--card);
      border:1px solid var(--border);
      border-radius:24px;
      padding:3rem 2rem;
      margin:4rem auto;
      max-width:600px;
      text-align:center;
    }
    .join-section h2 {
      color:var(--accent);
      margin-bottom:1.5rem;
      font-size:2.2rem;
    }
    input, button {
      width:100%;
      padding:16px;
      margin:10px 0;
      border-radius:12px;
      border:none;
      font-size:1.1rem;
    }
    input {
      background:#1e1e2e;
      color:white;
      border:1px solid #333;
    }
    input:focus { outline:2px solid var(--accent); }
    .btn-join {
      background:var(--accent);
      color:#000;
      font-weight:bold;
      cursor:pointer;
      font-size:1.2rem;
      transition:0.3s;
    }
    .btn-join:hover {
      background:#00cc7a;
      transform:scale(1.03);
    }

    /* Social Buttons */
    .social-buttons {
      display:flex;
      gap:1.5rem;
      justify-content:center;
      margin:3rem 0;
      flex-wrap:wrap;
    }
    .social-btn {
      display:flex;
      align-items:center;
      gap:12px;
      background:#1e1e2e;
      color:white;
      padding:16px 32px;
      border-radius:50px;
      text-decoration:none;
      font-weight:bold;
      font-size:1.1rem;
      transition:0.3s;
      border:1px solid #333;
    }
    .social-btn:hover {
      background:var(--accent);
      color:#000;
      transform:translateY(-5px);
    }
    .social-btn i { font-size:1.8rem; }

    footer {
      text-align:center;
      padding:3rem 0;
      color:var(--muted);
      border-top:1px solid #222;
    }

    /* Responsive HP */
    @media(max-width:768px){
      h1{font-size:2.5rem;}
      header{padding:4rem 0 3rem;}
      .join-section{padding:2rem 1.5rem;}
      .social-buttons{flex-direction:column; align-items:center;}
      .social-btn{width:90%; justify-content:center;}
    }
  </style>
</head>
<body>

  <header>
    <div class="container">
      <h1>CryptoNesia</h1>
      <p class="subtitle">Komunitas Crypto #1 Indonesia • Signal Akurat • Edukasi • Airdrop</p>
    </div>
  </header>

  <div class="container features">
    <div class="card">
      <i class="fas fa-chart-line"></i>
      <h3>Signal VIP Harian</h3>
      <p>Accuracy 90%+, entry & exit presisi dari tim analis pro.</p>
    </div>
    <div class="card">
      <i class="fas fa-users"></i>
      <h3>50.000+ Member</h3>
      <p>Grup Telegram & Discord rame 24 jam nonstop.</p>
    </div>
    <div class="card">
      <i class="fas fa-graduation-cap"></i>
      <h3>Edukasi Gratis</h3>
      <p>Webinar, ebook, mentoring 1-on-1 untuk semua level.</p>
    </div>
  </div>

  <!-- Form Join Member -->
  <div class="join-section">
    <h2>Gabung Komunitas Sekarang!</h2>
    <p style="color:#ccc;margin-bottom:2rem;">Isi data di bawah, langsung masuk grup VIP gratis 3 hari</p>
    <form action="https://formspree.io/f/your-form-id" method="POST"> <!-- Ganti dengan link Formspree/Web3Forms kamu -->
      <input type="text" name="nama" placeholder="Nama Lengkap" required />
      <input type="email" name="email" placeholder="Email Aktif" required />
      <input type="text" name="whatsapp" placeholder="Nomor WhatsApp (08xx)" required />
      <button type="submit" class="btn-join">JOIN SEKARANG GRATIS</button>
    </form>
  </div>

  <!-- Social Links -->
  <div class="container social-buttons">
    <a href="https://t.me/cryptonesia" class="social-btn" target="_blank">
      <i class="fab fa-telegram"></i> Gabung Telegram
    </a>
    <a href="https://discord.gg/cryptonesia" class="social-btn" target="_blank">
      <i class="fab fa-discord"></i> Gabung Discord
    </a>
  </div>

  <footer>
    <div class="container">
      <p>© 2025 CryptoNesia - Komunitas Crypto Terbesar Indonesia</p>
      <p style="margin-top:1rem;color:#777;">Dibuat dengan ❤️ untuk trader Indonesia</p>
    </div>
  </footer>

</body>
</html>
