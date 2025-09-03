<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Dashboard Kesehatan & Olahraga</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <aside class="sidebar">
    <h2>Menu</h2>
    <ul>
      <li><a href="#ringkasan">Ringkasan</a></li>
      <li><a href="#catatan">Catatan & Artikel</a></li>
      <li><a href="#tips">Inspirasi & Tips</a></li>
      <li><a href="#jadwal">Jadwal & Target</a></li>
    </ul>
  </aside>
  <main>
    <header>
      <h1>Dashboard Kesehatan & Olahraga</h1>
    </header>
    <section id="ringkasan">
      <h2>Ringkasan Hari Ini</h2>
      <div class="stats">
        <div>Langkah: <span id="steps">7500</span></div>
        <div>Kalori: <span id="calories">250</span></div>
        <div>Waktu Olahraga: <span id="exercise">30 menit</span></div>
      </div>
    </section>
    <section id="catatan">
      <h2>Catatan & Artikel</h2>
      <textarea placeholder="Tulis artikel atau catatan Anda di sini..."></textarea>
      <button id="saveNote">Simpan</button>
      <div id="notesList"></div>
    </section>
    <section id="tips">
      <h2>Inspirasi & Tips</h2>
      <div id="tipBox"></div>
    </section>
    <section id="jadwal">
      <h2>Jadwal & Target</h2>
      <input type="date" id="scheduleDate">
      <input type="text" id="scheduleText" placeholder="Target atau aktivitas">
      <button id="addSchedule">Tambah</button>
      <ul id="scheduleList"></ul>
    </section>
  </main>
  <script src="app.js"></script>
</body>
</html>
