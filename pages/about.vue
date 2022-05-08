<template>
    <div style="background-image: url(/wave-web.png)" class="bg-contain bg-no-repeat">
        <Navbar />
        <div class="flex flex-col m-28 p-20 bg-white shadow-xl rounded-md">
            <h1 class="text-4xl text-center font-extrabold text-gray-900 sm:text-3xl md:text-6xl">
                Profil Perusahaan
            </h1>
            <div class="flex flex-col mt-20 space-y-10">
                <ItemData v-for="item in datas" :key="item.name" :data="item"/>
            </div>
        </div>
    </div>
</template>

<script>
const datas = [
    {name: 'Nama Perusahaan', desc: 'PT TIRTA PERSADA ENVIRO'},
    {name: 'Direktur', desc: 'Basuki Cipto R. ST. MT'},
    {name: 'Alamat Kantor', desc: 'Jalan Raya ijen No 58. Kelurahan Wates, Kecamatan Magersari, Kota Mojokerto'},
    {name: 'Telepon', desc: '0811 3100 998'},
    {name: 'E-Mail', desc: 'tirtapersadaenviro@gmail.com'},
    {name: 'No NPWP', desc: '92.653.238.3-602.000'}
]

export default {
    data() {
        return {
            datas
        }
    },
}
</script>