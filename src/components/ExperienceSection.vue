<template>
  <section class="bg-gray-50 py-16 px-6 text-gray-800">
    <div class="max-w-4xl mx-auto">
      <h2 class="text-3xl font-bold mb-10 text-center">Riwayat Karier</h2>
      <div class="grid gap-6">
        <div v-for="item in experiences" :key="item.id" class="bg-white p-6 rounded-md shadow-md">
          <h3 class="text-xl font-semibold">{{ item.position }}</h3>
          <p class="text-sm text-gray-600">{{ item.company }} | {{ item.year }}</p>
          <p class="mt-2">{{ item.desc }}</p>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
const experiences = [
  { id: 1, position: 'Sales Freelance Product', company: 'PT. BASARI ANEKA KREASI / JAVABICA', year: '2019 – Sekarang', desc: 'Distribusi produk Delonghi, Franke, dan Gaggia secara fleksibel dan mandiri.' },
  { id: 2, position: 'Sales Tradisional Market', company: 'PT. MULTIMAYAKA', year: '2016 – Sekarang', desc: 'Menangani distribusi langsung ke toko dan mitra tradisional di seluruh Indonesia.' },
  { id: 3, position: 'SPV Sales Nasional', company: 'PT. MULTIMAYAKA', year: '2013 – 2016', desc: 'Memimpin tim SPG/SPB di Modern Market secara nasional dan menyusun strategi penjualan.' },
  { id: 4, position: 'SPV Admin Security', company: 'Hotel Alexis Jakarta', year: '2009 – 2011', desc: 'Mengatur operasional keamanan dan administrasi personel security hotel.' },
  { id: 5, position: 'Head Cashier', company: 'Kidzania Jakarta', year: '2007 – 2009', desc: 'Mengatur seluruh proses transaksi dan laporan penjualan harian.' },
  { id: 6, position: 'Purchasing', company: 'PT. Bumera Sakti Jaya', year: '2003 – 2006', desc: 'Bertanggung jawab atas pembelian dan pengadaan bahan baku.' },
  { id: 7, position: 'Cashier', company: 'PT. Indocater', year: '1994 – 1995', desc: 'Melayani transaksi dan membuat laporan penjualan harian.' }
]
</script>
