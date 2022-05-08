<template>
    <div>
        <Navbar/>
        <div>
            <div class="p-20 bg-blue-200">
                <h1 class="text-4xl text-center font-extrabold text-gray-900 sm:text-3xl md:text-6xl">
                    Klien Kami
                </h1>
                <p class="text-lg text-center pt-10">List perusahaan dan instansi yang pernah bekerja sama dengan kami</p>
            </div>
            <ol class="p-20 list-disc">
                <li v-for="(item, index) in clients" :key="index" class="text-lg">{{ item }}</li>
            </ol>
            <p class="px-20"><strong>* Dan masih banyak yang belum kami cantumkan</strong></p>
        </div>
    </div>
</template>

<script>
const clients = [
    'Pembangunan IPAL RS. Sido Waras – Kab. Mojokerto (20 m3/hari) - 2004',
    'Pembangunan IPAL RS. Jasem – Kab. Sidoarjo ( 20 m3/hari) - 2006',
    'Perencanan IPAL Puskesmas Gelora, Mentikan, dan Kedundung – Kota Mojokerto (10 m3/hari) - 2006',
    'Perencanaan IPAL RS. Dharma Husada – Kab. Mojokereto (10 m3/hari) - 2007',
    'Konsultan teknik pengoperasian IPAL PT. Mertex Indonesia – Kab. Mojokerto (2.500 m3/hari)',
    'Pembuatan incenerator di Dinas Kesehatan Kota Mojokerto - 2007',
    'Pembangunan IPAL PT. Dana Paint Indonesia – Sukodono – Kab. Sidoarjo -2008',
    'Perencanaan IPAL RSI. Sakinah – Kab. Mojokerto – 2008',
    'Pembangunan IPAL RS. Mawaddah Medika – Kab. Mojokerto – 2009',
    'Perencanaan IPAL PT. Satria Graha Sampurna – Krian Sidoarjo',
    'Perencanaan STP Hotel IBIS Jl. Basuki Rahmat Surabaya',
    'Pembangunan IPAL PT. Sumber Alam Indonesia – Jetis – Kab. Mojokerto (120 m3/ Hari) - 2010',
    'Perencanaan WWTP PT. Dharmala Intiland (3.000 m3/day) - 2014',
    'PT. Suprama Sidoarjo, industri makanan (200 m3/day) - 2016',
    'PT. Putra Mandiri Intipack Industri Pengolaan Plastik, Kecamatan Balongbendo, Kabupaten Sidoarjo',
    'Pembangunan IPAL PT. Aneka Kencana Plastindo, Industri Plastik - Kabupaten Sidoarjo (10 m3/hari) - 2019 ',
    'Pembangunan IPAL Taman Rekreasi Selecta Batu Malang (250 m3/day) - 2019 ',
    'Pembangunan IPAL PT Hui Xin, industri terpal - Surabaya (20 m3/day) - 2019 ',
    'Pembangunan IPAL CV. Jaya Abadi Plastik, Industri Rafia Jombang (100 m3/hari) - 2019',
    'Pembangunan Klinik Laboratorium Utama - Jenggolo Sidoarjo (2m3/hari) - 2019',
    'Penyusunan Dokumen UKL-UPL PT. Berkah berlimpah - 2019',
    'Penyusunan Dokumen DPLH CV Alpha Akasia - 2019',
    'Penyusunan Dokumen UKL-UPL PT DIC - 2019',
    'Pembangunan Klinik Krisna, Gresik (3 m3/hari) - 2019',
    'Penyusunan Dokumen UKL-UPL PT. TATA BERSAMA - Mojokerto - 2020',
    'Maintenance IPAL PT Dingsheng metal Indonesia, 2020',
    'Pengurusan IPLC Lab Jenggolo - Sidoarjo - 2020',
    'Pengurusan IPLC Pavillion Apartment - 2020',
    'Pengurusan IPLC Swiss Bel Hotel - 2020',
    'Pengurusan IPLC Aston Hotel - 2020',
    'Maintenance RS Baptis Batu - Malang (60 m3/hari) - 2020',
    'Perencanaan maintenance RS Aminah - Blitar - 2020',
    'Perencanaan maintenance RS Budi Rahayu - Blitar',
    'Perencanaan maintenance RS Dian Husada - 2020',
    'Pembuatan IPAL PT. Graha Mutu Persada (2 m3/hari) - 2020',
    'Pembuatan IPAL klinik CV. AZZKA Candi (3 m3/hari) - 2020',
    'Perencanaan Maintenance IPAL RS Kartini - 2020',
    'Maintenance RS Metro Cikupa Tangerang - 2020',
    'Pembuatan STP Siloam Hospital (30 m3/hari) - 2021',
    'Pembuatan STP Klinik Mediska Gubeng (3 m3/hari) - 2021',
    'Penyusunan Dokumen SPPL & Pertek PT AZZKA Candi - 2021',
    'Pengurusan SIPA PT. SGI Pasuruan - 2021',
    'Pengurusan SIPA PT. PRESTASI Ngoro Mojokerto - 2021',
    'Maintenance IPAL PT. SINAR RAYA, Pandaan Pasuruan - 2021 ',
    'Pembuatan IPAL PT. Lab. Fortuna Sampang (500 lt/hari) - 2021',
    'Pembuatan IPAL PT. Lab. Fortuna Sumenep (3 M3/hari) - 2021',
    'Pembuatan IPAL PT. Lab. Fortuna Lamongan (500 lt/hari) - 2021',
    'Pembuatan IPAL PT. Lab. Fortuna Bojonegoro (500 Lt/hari) - 2021',
    'Pembuatan IPAL PT. HOKKAN DELTAPACK , Mojokerto (15 m3/hari) - 2021',
    'Pembuatan IPAL PT. HOKKAN DELTAPACK, Sidoarjo (5 m3/hari) - 2021',
    'Pembuatan IPAL PT. KRISNA MAJU MAKMUR, Sidoarjo (8 m3/hari) - 2021',
    'Pembuatan IPAL PT. TRIJAYA, Sidoarjo (3 m3/hari) - 2021',
    'Pembuatan IPAL PT. KAMILA, Sidoarjo (3 m3/hari) - 2021',
    'Pembuatan IPAL UD SAHABAT, Mojosari Mojokerto, (30 m3/hari) 2021',
    'Maintenance IPAL RS SILOAM - Banjarmasin (40 m3/hr) - 2021',
    'Pengurusan Dokumen Lingkungan UD Sahabat Mojosari - Mojokerto - 2021',
    'Pengurusan Dokumen Lingkungan PT. TRIJAYA - Sidoarjo - 2021',
    'Pengurusan Dokumen Lingkungan PT. KAMILA - Sidoarjo - 2021',
    'Pengurusan Dokumen SLO IPAL RS. SILOAM - Mampang - 2021',
    'Pengurusan Dokumen SLO IPAL Apartemen Caspian - Surabaya - 2021',
]

export default {
    data() {
        return {
            clients
        }
    },
}
</script>