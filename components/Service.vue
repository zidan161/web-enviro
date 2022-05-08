<template>
    <div class="flex flex-col relative items-center">
        <img src="/bubble2.png" alt="" class="h-20 absolute top-28 right-40 lg:right-56">
        <img src="/bubble3.png" alt="" class="h-20 absolute lg:top-10 lg:left-56 bottom-20 left-10">
        <h1 class="text-4xl font-extrabold text-gray-900 mb-7 lg:text-6xl">
            Pelayanan Kami
        </h1>
        <div class="grid lg:grid-cols-3 sm:grid-cols-1 gap-7 mt-14 px-10">
            <ItemPoint v-for="item in services" :key="item" :service="item"/>
        </div>
        <div class="grid lg:grid-cols-2 sm:grid-cols-1 mt-7 gap-7 px-10">
            <ItemPoint v-for="item in service2" :key="item" :service="item"/>
        </div>
    </div>
</template>

<script>
const services = [ 
    'Problem Analysis', 
    'Design, Construction & Instalation',
    'Commissioning And Training',
]

const service2 = [
    'Operating And Maintenance',
    'Konsultan Dokumen Lingkungan',
]

export default {
    data() {
        return {
            services,
            service2
        }
    }
}
</script>