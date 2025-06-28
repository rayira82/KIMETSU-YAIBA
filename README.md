<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Kimetsu World: Petualangan Tanpa Akhir</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <link href="https://fonts.googleapis.com/css2?family=Unbounded&family=Cinzel:wght@700&display=swap" rel="stylesheet">
  <style>
    body {
      font-family: 'Unbounded', sans-serif;
      background-image: url('https://i.imgur.com/qRKiilX.jpeg'); /* Ganti ini kalau mau gambar lain */
      background-size: cover;
      background-position: center;
      background-attachment: fixed;
    }
    .overlay::before {
      content: "";
      position: fixed;
      top: 0; left: 0; right: 0; bottom: 0;
      background-color: rgba(0, 0, 0, 0.88);
      z-index: -1;
    }
    .judul-fantasi {
      font-family: 'Cinzel', serif;
      background: linear-gradient(to right, #a855f7, #ec4899, #ef4444);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
    }
  </style>
</head>
<body class="text-gray-100 overlay">

  <!-- HEADER -->
  <header class="text-center py-10">
    <h1 class="text-4xl md:text-5xl font-bold judul-fantasi">
      ✦ Dunia Kimetsu no Yaiba ✦
    </h1>
    <p class="mt-2 text-xl text-gray-300">Petualangan Tanpa Akhir</p>
    <div class="mt-3 mx-auto w-48 h-1 bg-gradient-to-r from-pink-500 to-purple-500 rounded-full shadow-lg"></div>
  </header>

  <!-- MAIN CONTENT -->
  <main class="max-w-3xl mx-auto px-4 space-y-6 pb-16">
    <p class="text-center text-sm text-gray-400">Klik judul bab untuk membuka ceritanya</p>

    <!-- BAB INTERAKTIF -->
    <div class="space-y-4">
      <!-- Bab Template -->
      <div class="bg-black bg-opacity-60 rounded-md">
        <button onclick="toggleContent('bab1')" class="w-full text-left text-blue-300 px-4 py-3 font-bold">📘 Bab 1: Awal Mula Petualangan</button>
        <div id="bab1" class="px-4 pb-4 hidden">
          <p>Tanjiro tinggal di desa kecil bersama keluarganya. Namun segalanya berubah ketika iblis menyerang, meninggalkan hanya dia dan Nezuko yang berubah menjadi iblis.</p>
        </div>
      </div>

      <div class="bg-black bg-opacity-60 rounded-md">
        <button onclick="toggleContent('bab2')" class="w-full text-left text-blue-300 px-4 py-3 font-bold">📘 Bab 2: Pertemuan dengan Giyu Tomioka</button>
        <div id="bab2" class="px-4 pb-4 hidden">
          <p>Tanjiro bertemu Giyu Tomioka, yang melihat potensi dalam dirinya dan membimbingnya menjadi pemburu iblis.</p>
        </div>
      </div>

      <div class="bg-black bg-opacity-60 rounded-md">
        <button onclick="toggleContent('bab3')" class="w-full text-left text-blue-300 px-4 py-3 font-bold">📘 Bab 3: Pertarungan Melawan Iblis</button>
        <div id="bab3" class="px-4 pb-4 hidden">
          <p>Bersama Nezuko, Zenitsu, dan Inosuke, Tanjiro menghadapi berbagai iblis kuat dan mulai memahami dunia baru yang mengerikan.</p>
        </div>
      </div>

      <div class="bg-black bg-opacity-60 rounded-md">
        <button onclick="toggleContent('bab4')" class="w-full text-left text-blue-300 px-4 py-3 font-bold">📘 Bab 4: Menghadapi Lawan yang Kuat</button>
        <div id="bab4" class="px-4 pb-4 hidden">
          <p>Mereka harus menghadapi Dua Belas Kizuki, kelompok iblis elit dengan kekuatan luar biasa dan taktik yang kejam.</p>
        </div>
      </div>

      <div class="bg-black bg-opacity-60 rounded-md">
        <button onclick="toggleContent('bab5')" class="w-full text-left text-blue-300 px-4 py-3 font-bold">📘 Bab 5: Pertempuran Akhir</button>
        <div id="bab5" class="px-4 pb-4 hidden">
          <p>Pertarungan melawan Muzan Kibutsuji menjadi penentu nasib manusia. Semua kekuatan dikerahkan untuk kemenangan terakhir.</p>
        </div>
      </div>

      <div class="bg-black bg-opacity-60 rounded-md">
        <button onclick="toggleContent('kesimpulan')" class="w-full text-left text-blue-300 px-4 py-3 font-bold">💬 Kesimpulan</button>
        <div id="kesimpulan" class="px-4 pb-4 hidden">
          <p>Kimetsu no Yaiba adalah kisah tentang keberanian, pengorbanan, dan harapan. Perjalanan Tanjiro menunjukkan bahwa cinta dan tekad bisa melawan kegelapan.</p>
        </div>
      </div>
    </div>
  </main>

  <!-- FOOTER -->
  <footer class="text-center py-6 text-gray-400 text-sm">
    © 2025 Kimetsu World Fan Page — Bukan situs resmi Kimetsu no Yaiba.
  </footer>

  <!-- SCRIPT TOGGLE -->
  <script>
    function toggleContent(id) {
      const el = document.getElementById(id);
      el.classList.toggle('hidden');
    }
  </script>
</body>
</html>
