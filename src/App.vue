<template>
  <!-- BACKGROUND GRADASI PASTEL CERAH SESUAI WHATSAPP IMAGE 2026-07-01 AT 10.53.56.JPEG -->
  <div class="min-h-screen bg-gradient-to-b from-rose-200 via-amber-100 to-sky-200 text-slate-800 font-sans antialiased">
    
    <!-- NAVBAR (Navigasi memanggil fungsi custom scrollToSection agar velocity lebih mantap) -->
    <nav class="sticky top-0 z-50 bg-white/20 backdrop-blur-md border-b border-black/5">
      <div class="max-w-5xl mx-auto px-6 h-16 flex items-center justify-between">
        <span class="font-bold text-xl tracking-wider text-slate-900">FARAH FITRIA.</span>
        <div class="hidden md:flex space-x-6 text-xs font-semibold text-slate-700">
          <button @click="scrollToSection('tentang')" class="hover:text-rose-600 transition duration-300 cursor-pointer">Tentang</button>
          <button @click="scrollToSection('kompetensi')" class="hover:text-rose-600 transition duration-300 cursor-pointer">Kompetensi</button>
          <button @click="scrollToSection('pengalaman')" class="hover:text-rose-600 transition duration-300 cursor-pointer">Pengalaman</button>
          <button @click="scrollToSection('pendidikan')" class="hover:text-rose-600 transition duration-300 cursor-pointer">Pendidikan</button>
          <button @click="scrollToSection('organisasi')" class="hover:text-rose-600 transition duration-300 cursor-pointer">Organisasi & Prestasi</button>
          <button @click="scrollToSection('kontak')" class="hover:text-rose-600 transition duration-300 cursor-pointer">Kontak</button>
        </div>
      </div>
    </nav>

    <!-- HERO SECTION -->
    <header id="tentang" class="max-w-5xl mx-auto px-6 py-12 md:py-20 grid md:grid-cols-12 gap-8 items-center overflow-hidden">
      <div class="md:col-span-7 text-center md:text-left order-2 md:order-1">
        <span class="inline-block bg-rose-500/10 backdrop-blur-sm text-rose-700 text-xs font-bold tracking-widest uppercase px-3 py-1 rounded-full mb-4 border border-rose-500/20">
          💡 FOOD TECHNOLOGY & CULINARY
        </span>
        <h1 class="text-4xl md:text-6xl font-black text-white tracking-tight mb-4">
          Halo, saya <span class="bg-gradient-to-r from-rose-600 to-orange-500 bg-clip-text text-transparent">Farah Fitria Amalia</span>
        </h1>
        <p class="text-sm font-bold text-slate-600 uppercase tracking-wider mb-4">
          Food Technology • Culinary • R&D • Food Safety • Nutrition
        </p>
        <p class="text-slate-800 text-sm leading-relaxed mb-8 text-justify bg-white/40 p-5 rounded-2xl border border-white/60 backdrop-blur-sm shadow-md">
          Farah Fitria Amalia merupakan mahasiswa Teknologi Pangan di Universitas Sahid Jakarta dengan latar belakang pendidikan Tata Boga pada tingkat SMK. Memiliki minat besar dalam bidang kuliner dan pengolahan pangan, serta kemampuan bekerja di laboratorium kimia dan mikrobiologi yang didukung oleh pengetahuan akademik di bidang teknologi pangan. Saya merupakan pribadi yang memiliki antusiasme tinggi terhadap hal-hal baru, terutama dalam bidang food and beverage, serta berkomitmen untuk terus belajar dan mengembangkan kompetensi.
        </p>
        <div class="flex flex-wrap gap-4 justify-center md:justify-start">
          <button @click="scrollToSection('pengalaman')" class="bg-gradient-to-r from-rose-500 to-orange-500 text-white px-6 py-3 rounded-full font-bold shadow-lg shadow-rose-500/20 hover:opacity-90 transition duration-300 cursor-pointer">Lihat Portofolio →</button>
          <button @click="scrollToSection('kontak')" class="bg-black/5 backdrop-blur-sm border border-black/10 text-slate-800 px-6 py-3 rounded-full font-medium hover:bg-black/10 transition duration-300 cursor-pointer">Informasi Kontak</button>
        </div>
      </div>
      
      <!-- FOTO SEBELAH KANAN MASKING TRANSPARAN -->
      <div class="md:col-span-5 flex justify-center md:justify-end order-1 md:order-2 mb-8 md:mb-0">
        <div class="relative w-full max-w-sm md:max-w-md flex justify-center items-center drop-shadow-[0_25px_35px_rgba(231,113,133,0.3)] animate-hero-appearance">
          <img 
            src="/hero.png" 
            alt="Farah Fitria Amalia" 
            class="w-full h-auto object-contain scale-90 md:scale-100 origin-bottom transition-transform duration-750 ease-out hover:scale-[1.03]"
            style="-webkit-mask-image: linear-gradient(to top, transparent 0%, black 25%); mask-image: linear-gradient(to top, transparent 0%, black 25%);"
          />
        </div>
      </div>
    </header>

    <!-- LAYANAN & KEAHLIAN / KOMPETENSI -->
    <section id="kompetensi" class="max-w-5xl mx-auto px-6 py-12">
      <h2 class="text-2xl font-bold text-slate-900 mb-8 flex items-center gap-2">
        <span class="h-6 w-1 bg-rose-500 inline-block rounded-full"></span> Kompetensi Utama
      </h2>
      <div class="grid md:grid-cols-3 gap-6 mb-8">
        <div class="bg-white/40 backdrop-blur-md p-6 rounded-3xl border border-white/60 shadow-md">
          <div class="text-2xl mb-3">✨</div>
          <h3 class="font-bold text-slate-900 text-lg mb-2">Product Development (R&D)</h3>
          <p class="text-xs text-slate-700 leading-relaxed">Inovasi dan formulasi resep produk pangan baru menggabungkan keahlian boga & pendekatan sains.</p>
        </div>
        <div class="bg-white/40 backdrop-blur-md p-6 rounded-3xl border border-white/60 shadow-md">
          <div class="text-2xl mb-3">🛡️</div>
          <h3 class="font-bold text-slate-900 text-lg mb-2">Food Safety (HACCP & GMP)</h3>
          <p class="text-xs text-slate-700 leading-relaxed">Implementasi jaminan mutu produk, standar HACCP, GMP, serta regulasi pangan & halal industri F&B.</p>
        </div>
        <div class="bg-white/40 backdrop-blur-md p-6 rounded-3xl border border-white/60 shadow-md">
          <div class="text-2xl mb-3">🔬</div>
          <h3 class="font-bold text-slate-900 text-lg mb-2">Lab Analysis</h3>
          <p class="text-xs text-slate-700 leading-relaxed">Pengujian berkala sampel bahan baku dan produk jadi secara mikrobiologi (AKK, Uji ALT) & kimiawi laboratorium.</p>
        </div>
      </div>

      <!-- MATRIKS SKILLS -->
      <div class="grid md:grid-cols-3 gap-6">
        <div class="bg-white/30 p-5 rounded-2xl border border-white/40 shadow-sm">
          <h4 class="font-bold text-xs uppercase tracking-wider text-rose-700 mb-3">Technical Skills</h4>
          <ul class="text-xs text-slate-700 space-y-1.5 list-disc pl-4">
            <li>Product Development (R&D)</li>
            <li>Food Safety (HACCP & GMP)</li>
            <li>Lab Analysis (Microbiology & Kimia)</li>
            <li>Food Regulation & Halal</li>
            <li>Cook Helper (Pastry bakery & Hot Kitchen)</li>
          </ul>
        </div>
        <div class="bg-white/30 p-5 rounded-2xl border border-white/40 shadow-sm">
          <h4 class="font-bold text-xs uppercase tracking-wider text-rose-700 mb-3">Software & Tools</h4>
          <ul class="text-xs text-slate-700 space-y-1.5 list-disc pl-4">
            <li>Microsoft Office & Excel (Data Analysis, Pivot Table)</li>
            <li>Canva (Desain Grafis Visual Content)</li>
            <li>Manajemen Waktu & Bekerja Secara Tim</li>
          </ul>
        </div>
        <div class="bg-white/30 p-5 rounded-2xl border border-white/40 shadow-sm">
          <h4 class="font-bold text-xs uppercase tracking-wider text-rose-700 mb-3">Laboratory Tools</h4>
          <ul class="text-xs text-slate-700 space-y-1.5 list-disc pl-4">
            <li>Spectrophotometer</li>
            <li>pH Meter</li>
            <li>Autoclave</li>
          </ul>
        </div>
      </div>
    </section>

    <!-- PENGALAMAN KERJA -->
    <section id="pengalaman" class="max-w-5xl mx-auto px-6 py-12">
      <h2 class="text-2xl font-bold text-slate-900 mb-8 flex items-center gap-2">
        <span class="h-6 w-1 bg-rose-500 inline-block rounded-full"></span> Pengalaman Kerja
      </h2>
      <div class="space-y-6">
        
        <!-- PT SOLUSI NUTRI SEHAT -->
        <div class="bg-white/50 backdrop-blur-md p-6 rounded-3xl border-2 border-rose-300 shadow-lg relative overflow-hidden">
          <div class="absolute top-0 right-0 bg-rose-500 text-white font-bold text-[10px] tracking-widest uppercase px-3 py-1 rounded-bl-xl">
            
          </div>
          <div class="flex flex-wrap justify-between items-start gap-2">
            <div>
              <h3 class="font-bold text-lg text-slate-900">Product Operation and Development</h3>
              <p class="text-xs font-semibold text-slate-600">PT Solusi Nutri Sehat — Jakarta, Indonesia</p>
            </div>
            <span class="text-xs font-bold text-rose-700 bg-rose-500/10 px-2.5 py-1 rounded-full border border-rose-500/20">Juni 2026</span>
          </div>
          <ul class="text-xs text-slate-700 mt-3 list-disc pl-4 space-y-1">
            <li>Melakukan Quality Control pada saat proses pembuatan produk mulai dari bahan baku datang hingga pengemasan.</li>
            <li>Menjaga Kebersihan ruang produksi dengan menjadwalkan General cleaning dan deep cleaning di area produksi.</li>
            <li>Membuat list bahan baku yang telah habis dan memastikan stok di gudang terpenuhi.</li>
            <li>Membuat KPI setiap bulan sekali.</li>
          </ul>
        </div>

        <!-- SAJA GROUP -->
        <div class="bg-white/40 backdrop-blur-md p-6 rounded-3xl border border-white/60 shadow-md">
          <div class="flex flex-wrap justify-between items-start gap-2">
            <div>
              <h3 class="font-bold text-lg text-slate-900">Internship (Pastry)</h3>
              <p class="text-xs font-semibold text-slate-600">SAJA Group — Jakarta, Indonesia</p>
            </div>
            <span class="text-xs font-bold text-slate-600 bg-black/5 px-2.5 py-1 rounded-full border border-black/10">Mar 2026 – Apr 2026</span>
          </div>
          <ul class="text-xs text-slate-700 mt-3 list-disc pl-4 space-y-1">
            <li>Berperan sebagai commis chef dengan membatu menimbang bahan baku untuk pembuatan produk seperti cookies, cake, puding dan beberapa produk pastry.</li>
            <li>Membuat produk dari awal sampai akhir dan mengecek kembali orderan yang diterima.</li>
            <li>Mencatat bahan baku yang sudah habis dan mengordernya ke tim gudang.</li>
            <li>Menjalankan live cooking di event tertentu.</li>
          </ul>
        </div>

        <!-- SIDO MUNCUL -->
        <div class="bg-white/40 backdrop-blur-md p-6 rounded-3xl border border-white/60 shadow-md">
          <div class="flex flex-wrap justify-between items-start gap-2">
            <div>
              <h3 class="font-bold text-lg text-slate-900">Internship (Analis Laboratorium Pangan)</h3>
              <p class="text-xs font-semibold text-slate-600">PT. Industri Jamu dan Farmasi Sido Muncul — Semarang, Jawa Tengah</p>
            </div>
            <span class="text-xs font-bold text-slate-600 bg-black/5 px-2.5 py-1 rounded-full border border-black/10">Sep 2025 – Oct 2025</span>
          </div>
          <ul class="text-xs text-slate-700 mt-3 list-disc pl-4 space-y-1">
            <li>Berpartisipasi dalam kegiatan pengujian bahan baku dan produk jadi di laboratorium kimia, meliputi uji logam berat, pengawet, vitamin B dan K, kurkumin, gingerol, serta saponin.</li>
            <li>Bertanggung jawab melakukan analisis mikrobiologi seperti uji AKK, ALT, dan personal hygiene untuk memastikan kualitas serta keamanan produk.</li>
            <li>Mempelajari secara langsung proses pengolahan produk mulai dari bahan baku hingga menjadi produk jadi yang siap dipasarkan.</li>
          </ul>
        </div>

        <!-- CARLINO BAKES -->
        <div class="bg-white/40 backdrop-blur-md p-6 rounded-3xl border border-white/60 shadow-md">
          <div class="flex flex-wrap justify-between items-start gap-2">
            <div>
              <h3 class="font-bold text-lg text-slate-900">Internship (Pastry)</h3>
              <p class="text-xs font-semibold text-slate-600">Carlino Bakes — Jakarta, Indonesia</p>
            </div>
            <span class="text-xs font-bold text-slate-600 bg-black/5 px-2.5 py-1 rounded-full border border-black/10">Apr 2022 – May 2022</span>
          </div>
          <ul class="text-xs text-slate-700 mt-3 list-disc pl-4 space-y-1">
            <li>Bertanggung jawab membantu chef dalam proses pembuatan produk, mulai dari menimbang gramasi bahan baku hingga tahap produksi.</li>
            <li>Mengolah berbagai jenis produk seperti pastry, cookies, dan goguma ppang (roti ubi khas Korea) dengan memperhatikan kualitas dan konsistensi rasa.</li>
            <li>Memastikan setiap pesanan terpenuhi tepat waktu serta menjaga kebersihan dan kerapian lingkungan kerja selama proses produksi.</li>
          </ul>
        </div>

        <!-- MILLENIUM HOTEL SIRIH -->
        <div class="bg-white/40 backdrop-blur-md p-6 rounded-3xl border border-white/60 shadow-md">
          <div class="flex flex-wrap justify-between items-start gap-2">
            <div>
              <h3 class="font-bold text-lg text-slate-900">Internship (Hot Kitchen)</h3>
              <p class="text-xs font-semibold text-slate-600">Millenium Hotel Sirih Jakarta — Jakarta, Indonesia</p>
            </div>
            <span class="text-xs font-bold text-slate-600 bg-black/5 px-2.5 py-1 rounded-full border border-black/10">Jun 2021 – Jul 2021</span>
          </div>
          <ul class="text-xs text-slate-700 mt-3 list-disc pl-4 space-y-1">
            <li>Membantu dalam persiapan dan pembuatan pesanan box sebanyak 1.000 pcs untuk kebutuhan event perusahaan.</li>
            <li>Bertanggung jawab menjaga stand makanan dan minuman saat breakfast tamu, serta memastikan seluruh hidangan tetap tersedia dan tersaji dengan baik.</li>
          </ul>
        </div>

        <!-- HOTEL GREN ALIA CIKINI -->
        <div class="bg-white/40 backdrop-blur-md p-6 rounded-3xl border border-white/60 shadow-md">
          <div class="flex flex-wrap justify-between items-start gap-2">
            <div>
              <h3 class="font-bold text-lg text-slate-900">Internship (Cook Helper)</h3>
              <p class="text-xs font-semibold text-slate-600">Hotel Gren Alia Cikini — Jakarta, Indonesia</p>
            </div>
            <span class="text-xs font-bold text-slate-600 bg-black/5 px-2.5 py-1 rounded-full border border-black/10">Jan 2021 – Jun 2021</span>
          </div>
          <ul class="text-xs text-slate-700 mt-3 list-disc pl-4 space-y-1">
            <li>Berperan sebagai cook helper dengan membantu persiapan bahan baku hingga proses pembuatan berbagai menu makanan.</li>
            <li>Membantu dalam pembuatan dan penyajian minuman, termasuk berbagai jenis kopi menggunakan mesin kopi serta minuman non-kopi lainnya.</li>
            <li>Bertanggung jawab dalam pembuatan dessert, mulai dari persiapan bahan baku hingga tahap plating agar hasil tampil menarik dan sesuai standar penyajian.</li>
          </ul>
        </div>
      </div>
    </section>

    <!-- PENDIDIKAN -->
    <section id="pendidikan" class="max-w-5xl mx-auto px-6 py-12">
      <h2 class="text-2xl font-bold text-slate-900 mb-8 flex items-center gap-2">
        <span class="h-6 w-1 bg-rose-500 inline-block rounded-full"></span> Riwayat Pendidikan
      </h2>
      <div class="grid md:grid-cols-2 gap-6">
        <div class="bg-white/50 backdrop-blur-md p-6 rounded-3xl border border-white shadow-md relative overflow-hidden">
          <div class="absolute top-0 right-0 bg-rose-500 text-white font-bold text-xs px-4 py-1.5 rounded-bl-2xl">
            🏆 IPK: 3.85 / 4.00
          </div>
          <span class="text-xs font-bold text-rose-700 block mb-1">Sep 2022 – Sekarang</span>
          <h3 class="text-xl font-bold text-slate-900">Universitas Sahid Jakarta</h3>
          <p class="text-xs font-semibold text-slate-600 mb-3">Mahasiswa Teknologi Pangan</p>
          <ul class="text-xs text-slate-700 space-y-1 list-disc pl-4 text-justify">
            <li>Aktif berorganisasi dan mampu bekerja sama secara efektif dalam penyusunan laporan analisis komprehensif (Nilai A).</li>
            <li>Menyelesaikan praktikum pengembangan produk dengan predikat A serta meraih Juara 1 Business Plan Dragonana Fruits Strip.</li>
            <li>Terlibat aktif dalam Program Kreativitas Mahasiswa (PKM) dan praktikum laboratorium.</li>
          </ul>
        </div>

        <div class="bg-white/50 backdrop-blur-md p-6 rounded-3xl border border-white shadow-md relative overflow-hidden">
          <div class="absolute top-0 right-0 bg-slate-700 text-white font-bold text-xs px-4 py-1.5 rounded-bl-2xl">
            Nilai: 88.00 / 100.00
          </div>
          <span class="text-xs font-bold text-slate-600 block mb-1">Aug 2019 – Oct 2022</span>
          <h3 class="text-xl font-bold text-slate-900">SMK Negeri 38 Jakarta</h3>
          <p class="text-xs font-semibold text-slate-600 mb-3">Jurusan Tata Boga</p>
          <ul class="text-xs text-slate-700 space-y-1 list-disc pl-4 text-justify">
            <li>Mengikuti kompetisi kuliner lokal (Pucung Betawi dan Fusion Food: Black Klepon dengan Salted Caramel).</li>
            <li>Berpartisipasi dalam kegiatan produksi dan manajemen penjualan roti sekolah.</li>
            <li>Meraih sertifikasi resmi LSP untuk klaster makanan kontinental, produk bakery, dan makanan indonesia.</li>
          </ul>
        </div>
      </div>
    </section>

    <!-- ORGANISASI, PRESTASI & SERTIFIKASI -->
    <section id="organisasi" class="max-w-5xl mx-auto px-6 py-12">
      <div class="grid md:grid-cols-2 gap-8">
        <div class="space-y-6">
          <h2 class="text-2xl font-bold text-slate-900 flex items-center gap-2">
            <span class="h-6 w-1 bg-rose-500 inline-block rounded-full"></span> Pengalaman Organisasi
          </h2>
          <div class="bg-white/40 p-6 rounded-3xl border border-white/60 shadow-md">
            <span class="text-xs font-bold text-rose-700">Sep 2024 – Apr 2025</span>
            <h3 class="font-bold text-base text-slate-900 mt-1">Sekretaris</h3>
            <p class="text-xs font-semibold text-slate-600 mb-2">Himpunan Mahasiswa Teknologi Pangan (HIMATEPA)</p>
            <ul class="text-xs text-slate-700 list-disc pl-4 space-y-1 text-justify">
              <li>Membuat surat-surat administrasi resmi untuk pengajuan dari awal hingga akhir acara.</li>
              <li>Menyusun rancangan proposal pengajuan sponsor kegiatan.</li>
              <li>Membuat dokumen rekapitulasi laporan hasil evaluasi bulanan organisasi.</li>
            </ul>
          </div>
        </div>

        <div class="space-y-6">
          <h2 class="text-2xl font-bold text-slate-900 flex items-center gap-2">
            <span class="h-6 w-1 bg-rose-500 inline-block rounded-full"></span> Kompetisi & Penghargaan
          </h2>
          <div class="space-y-4">
            <div class="bg-white/60 p-4 rounded-2xl border border-white flex gap-3">
              <span class="text-xl">🥇</span>
              <div>
                <h4 class="font-bold text-xs text-slate-900">Juara 1 Lomba Business Plan Competition (2025)</h4>
                <p class="text-[11px] text-slate-700">Inovasi Dragonana Fruits Strip dengan tema "Zero waste food processing solusi teknologi tepat untuk mengolah komoditi pangan lokal" — Universitas Sahid.</p>
              </div>
            </div>
            <div class="bg-white/60 p-4 rounded-2xl border border-white flex gap-3">
              <span class="text-xl">🥉</span>
              <div>
                <h4 class="font-bold text-xs text-slate-900">Juara 3 Lomba Business Plan (2025)</h4>
                <p class="text-[11px] text-slate-700">Tema "Produk Berbasis Kedelai" — Diselenggarakan oleh The US Soybean Export Council (USSEC), Universitas Sahid, dan Sandination.</p>
              </div>
            </div>
            <div class="bg-white/60 p-4 rounded-2xl border border-white flex gap-3">
              <span class="text-xl">🧬</span>
              <div>
                <h4 class="font-bold text-xs text-slate-900">Penerima Hibah Pendanaan PKM-RE (2024 & 2025)</h4>
                <p class="text-[11px] text-slate-700">Lolos seleksi ketat hibah riset eksakta nasional oleh KEMENDIKBUDRISTEK RI selama dua tahun berturut-turut.</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- KONTAK VIEW-ONLY CARDS -->
    <section id="kontak" class="max-w-5xl mx-auto px-6 py-16 mb-16">
      <div class="bg-white/40 backdrop-blur-md p-8 rounded-3xl border border-white/60 shadow-lg text-center max-w-2xl mx-auto">
        <h2 class="text-2xl font-bold text-slate-900 mb-2">Informasi Kontak</h2>
        <p class="text-xs text-slate-600 mb-8">Silakan tinjau profil profesional saya melalui detail resmi di bawah ini:</p>
        
        <div class="grid grid-cols-1 sm:grid-cols-2 gap-4 max-w-xl mx-auto text-left">
          <div class="bg-white/50 p-4 rounded-2xl border border-white/80 shadow-sm flex items-center gap-3">
            <span class="text-xl">✉️</span>
            <div>
              <p class="text-[10px] font-bold text-rose-700 uppercase tracking-wider">Email</p>
              <p class="text-xs font-semibold text-slate-800">farahhhfitria@gmail.com</p>
            </div>
          </div>

          <div class="bg-white/50 p-4 rounded-2xl border border-white/80 shadow-sm flex items-center gap-3">
            <span class="text-xl">📞</span>
            <div>
              <p class="text-[10px] font-bold text-rose-700 uppercase tracking-wider">WhatsApp</p>
              <p class="text-xs font-semibold text-slate-800">088210338174</p>
            </div>
          </div>

          <div class="bg-white/50 p-4 rounded-2xl border border-white/80 shadow-sm flex items-center gap-3 sm:col-span-2">
            <span class="text-xl">🔗</span>
            <div class="overflow-hidden">
              <p class="text-[10px] font-bold text-rose-700 uppercase tracking-wider">LinkedIn</p>
              <p class="text-xs font-semibold text-slate-800 truncate">linkedin.com/in/farah-fitria-amalia-239361227</p>
            </div>
          </div>

          <div class="bg-white/50 p-4 rounded-2xl border border-white/80 shadow-sm flex items-start gap-3 sm:col-span-2">
            <span class="text-xl mt-0.5">📍</span>
            <div>
              <p class="text-[10px] font-bold text-rose-700 uppercase tracking-wider">Alamat Rumah</p>
              <p class="text-xs font-semibold text-slate-800 leading-relaxed">
                Jalan Madrasah II Nomor 54, RT 01/RW 02, Kelurahan Sukabumi Utara, Kecamatan Kebon Jeruk, Kota Administrasi Jakarta Barat, DKI Jakarta 11540.
              </p>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- FOOTER -->
    <footer class="bg-white/40 text-slate-500 text-xs py-8 text-center border-t border-black/5">
      <p>&copy; 2026 Farah Fitria Amalia. Crafted for Food & Beverage Industry Excellence.</p>
    </footer>

  </div>
</template>

<script setup>
// Fungsi kustom untuk transisi bergulir berkecepatan tinggi (high velocity easing)
const scrollToSection = (id) => {
  const element = document.getElementById(id);
  if (element) {
    const offset = 80; // Jarak kompensasi tinggi navbar
    const bodyRect = document.body.getBoundingClientRect().top;
    const elementRect = element.getBoundingClientRect().top;
    const elementPosition = elementRect - bodyRect;
    const offsetPosition = elementPosition - offset;

    // Pergerakan instan berkecepatan tinggi yang dikontrol halus lewat window.scrollTo
    window.scrollTo({
      top: offsetPosition,
      behavior: 'smooth'
    });
  }
};
</script>