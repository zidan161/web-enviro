<template>
    <div style="background-image: url(/wave-web.png)" class="py-24 flex flex-col space-y-10 px-20 bg-contain bg-no-repeat lg:flex-row lg:space-x-16 lg:space-y-0">
        <img src="/company.jpg" alt="image company" class="rounded-lg max-w-md">
        <div class="flex flex-col space-y-10">
            <h1 class="text-4xl font-extrabold text-gray-900 sm:text-4xl md:text-6xl">
                Jasa Layanan
            </h1>
            <div class="flex flex-col space-y-5">
                <ItemDoc v-for="doc in listDoc" :key="doc.name" :doc="doc"/>
            </div>
        </div>
    </div>
</template>

<script>
const listDoc = [
    {name: 'Konsultasi penyusunan dokumen AMDAL'},
    {name: 'Konsultasi penyusunan dokumen lingkungan UKL-UPL, SIPA, SLO IPAL, TPS B3 Dll'},
    {name: 'Konsultasi dan pengurusan izin pembuangan limbah'},
    {name: 'Konsultasi untuk Penempatan dan Penyimpanan Bahan B3 dan Limbah B3'},
    {name: 'Penyusunan dokumen ANDALALIN'},
    {name: 'Perencanaan dan pembangunan konstruksi untuk penanganan limbah'},
]

export default {
    data() {
        return {
            listDoc
        }
    },
}
</script>
