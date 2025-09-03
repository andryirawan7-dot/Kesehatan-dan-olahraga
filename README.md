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
body {
  font-family: 'Segoe UI', Arial, sans-serif;
  margin: 0;
  background: #f6f8fc;
  display: flex;
}
.sidebar {
  background: #2e8b57;
  color: #fff;
  width: 220px;
  min-height: 100vh;
  padding: 24px 0;
  position: fixed;
}
.sidebar h2 {
  text-align: center;
  margin-bottom: 16px;
}
.sidebar ul {
  list-style: none;
  padding: 0;
}
.sidebar ul li {
  margin: 16px 0;
}
.sidebar ul li a {
  color: #fff;
  text-decoration: none;
  font-weight: bold;
}
main {
  margin-left: 240px;
  padding: 32px;
  flex: 1;
}
header h1 {
  color: #2e8b57;
  margin-bottom: 24px;
}
section {
  background: #fff;
  border-radius: 12px;
  padding: 24px;
  margin-bottom: 24px;
  box-shadow: 0 2px 8px rgba(44, 62, 80, .07);
}
.stats {
  display: flex;
  gap: 32px;
  font-size: 1.2em;
}
textarea {
  width: 100%;
  height: 80px;
  margin: 8px 0;
  border-radius: 8px;
  border: 1px solid #ccc;
  padding: 8px;
  resize: vertical;
}
button {
  background: #2e8b57;
  color: #fff;
  border: none;
  padding: 8px 20px;
  border-radius: 8px;
  cursor: pointer;
  margin-top: 8px;
}
button:hover {
  background: #246b43;
}
#notesList, #scheduleList {
  margin-top: 12px;
}
#tipBox {
  background: #e0f8ea;
  padding: 14px;
  border-radius: 8px;
  font-size: 1.1em;
  color: #246b43;
}
@media (max-width: 700px) {
  .sidebar {
    position: static;
    width: 100%;
    min-height: auto;
    padding: 12px 0;
  }
  main {
    margin-left: 0;
    padding: 8px;
  }
}
