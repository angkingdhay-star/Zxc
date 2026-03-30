# Zxc
zxc
<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>The Wedding of A & B</title>
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@500;700&family=Montserrat:wght@300;400;500&display=swap" rel="stylesheet">
<style>
  * {margin:0; padding:0; box-sizing:border-box;}
  body {
    font-family:'Montserrat', sans-serif;
    background-color:#f9f7f3;
    color:#4a3b2f;
    overflow-x:hidden;
  }
  section {
    width:100%;
    height:100vh;
    display:flex;
    flex-direction:column;
    justify-content:center;
    align-items:center;
    text-align:center;
    padding:2rem;
    position:relative;
  }
  h1, h2, h3 {
    font-family:'Playfair Display', serif;
    color:#3b2f2f;
  }
  .cover {
    background:linear-gradient(rgba(255,255,255,0.7),rgba(255,255,255,0.7)), url('foto-pasangan.jpg') center/cover no-repeat;
    backdrop-filter:blur(5px);
  }
  .cover h1 {
    font-size:2rem;
    letter-spacing:2px;
  }
  .cover h2 {
    font-size:1.5rem;
    margin:1rem 0;
  }
  .btn {
    background-color:#d4b483;
    color:white;
    padding:0.8rem 1.5rem;
    border:none;
    border-radius:30px;
    font-weight:500;
    margin-top:1.5rem;
    cursor:pointer;
    transition:all 0.3s ease;
  }
  .btn:hover {background-color:#c3a06b;}
  .quote {
    background-color:#fffaf3;
    background-image:url('floral-bg.png');
    background-size:cover;
  }
  .quote p {
    font-style:italic;
    margin-top:1rem;
    color:#6b5b4b;
  }
  .mempelai {
    background-color:#fdfbf8;
    display:flex;
    flex-direction:column;
    gap:1rem;
  }
  .mempelai img {
    width:120px;
    height:120px;
    border-radius:50%;
    object-fit:cover;
    border:2px solid #d4b483;
  }
  .save-date {
    background-color:#fffaf3;
  }
  .save-date h1 {
    font-size:2.5rem;
    color:#b89b6b;
  }
  .detail {
    background-color:#f9f7f3;
  }
  .detail .card {
    background:white;
    border-radius:10px;
    box-shadow:0 2px 8px rgba(0,0,0,0.1);
    padding:1rem;
    margin:1rem 0;
    width:80%;
  }
  .map {
    background-color:#fffaf3;
  }
  iframe {
    width:90%;
    height:300px;
    border:none;
    border-radius:10px;
  }
  .rsvp {
    background-color:#fdfbf8;
  }
  form {
    display:flex;
    flex-direction:column;
    gap:0.8rem;
    width:80%;
  }
  input, select {
    padding:0.7rem;
    border:1px solid #d4b483;
    border-radius:5px;
  }
  .footer {
    background-color:#fffaf3;
    font-size:0.9rem;
    color:#6b5b4b;
  }
  /* Animasi */
  [data-animate] {
    opacity:0;
    transform:translateY(30px);
    transition:all 0.8s ease;
  }
  [data-animate].visible {
    opacity:1;
    transform:translateY(0);
  }
</style>
</head>
<body>

<!-- COVER -->
<section class="cover" id="cover">
  <h1>The Wedding Of</h1>
  <h2>Ahmad & Bella</h2>
  <p>Kepada Yth. Bapak/Ibu/Saudara/i<br><strong>[Nama Tamu]</strong></p>
  <button class="btn" onclick="scrollToNext()">Open Invitation</button>
  <audio id="bgm" src="romantic-instrumental.mp3" autoplay loop></audio>
</section>

<!-- AYAT -->
<section class="quote" data-animate>
  <h2>QS. Ar-Rum: 21</h2>
  <p>وَمِنْ آيَاتِهِ أَنْ خَلَقَ لَكُم مِّنْ أَنفُسِكُمْ أَزْوَاجًا ...</p>
  <p>"Dan di antara tanda-tanda (kebesaran)-Nya ialah Dia menciptakan pasangan-pasangan untukmu..."</p>
</section>

<!-- MEMPELAI -->
<section class="mempelai" data-animate>
  <img src="pria.jpg" alt="Mempelai Pria">
  <h3>Ahmad Fauzan</h3>
  <p>Putra dari Bapak Fulan & Ibu Fulanah</p>
  <img src="wanita.jpg" alt="Mempelai Wanita">
  <h3>Bella Rahmawati</h3>
  <p>Putri dari Bapak Fulan & Ibu Fulanah</p>
</section>

<!-- SAVE THE DATE -->
<section class="save-date" data-animate>
  <h1>12 . 12 . 2026</h1>
  <h3>Save The Date</h3>
</section>

<!-- DETAIL ACARA -->
<section class="detail" data-animate>
  <div class="card">
    <h3>Akad Nikah</h3>
    <p>Sabtu, 12 Desember 2026<br>08.00 WIB<br>Masjid Al-Falah, Bandung</p>
  </div>
  <div class="card">
    <h3>Resepsi</h3>
    <p>Sabtu, 12 Desember 2026<br>11.00 WIB<br>Gedung Serbaguna Harmoni</p>
  </div>
</section>

<!-- MAP -->
<section class="map" data-animate>
  <h3>Lokasi Acara</h3>
  <iframe src="https://www.google.com/maps/embed?..."></iframe>
  <button class="btn">Lihat Lokasi</button>
</section>

<!-- RSVP -->
<section class="rsvp" data-animate>
  <h3>Konfirmasi Kehadiran</h3>
  <form>
    <input type="text" placeholder="Nama">
    <select>
      <option>Hadir</option>
      <option>Tidak Hadir</option>
    </select>
    <input type="number" placeholder="Jumlah Tamu">
    <button class="btn" type="submit">Kirim</button>
  </form>
</section>

<!-- PENUTUP -->
<section class="footer" data-animate>
  <p>Merupakan suatu kehormatan dan kebahagiaan bagi kami apabila Bapak/Ibu/Saudara/i berkenan hadir.</p>
  <p>Ahmad & Bella</p>
</section>

<script>
  function scrollToNext() {
    document.querySelector('#cover').nextElementSibling.scrollIntoView({behavior:'smooth'});
  }
  const observer = new IntersectionObserver(entries => {
    entries.forEach(entry => {
      if(entry.isIntersecting) entry.target.classList.add('visible');
    });
  }, {threshold:0.2});
  document.querySelectorAll('[data-animate]').forEach(el => observer.observe(el));
</script>

</body>
</html>
```
---
