<template>
    <div class="flex flex-col items-center">
        <h1 class="text-2xl font-extrabold text-gray-900 sm:text-4xl md:text-4xl">
            Our Service
        </h1>
        <p>kami menyediakan pelayan berikut</p>
        <div class="grid grid-cols-5 gap-4 mt-7">
            <ItemPoint v-for="item in services" :key="item.name" :service="item"/>
        </div>
    </div>
</template>

<script>
const loremIpsum = "Lorem ipsum dolor sit amet consectetur adipisicing elit. Maxime mollitia, molestiae quas vel sint commodi repudiandae consequuntur voluptatum laborum numquam blanditiis"

const services = [
    { name: 'Pemesanan', description: loremIpsum },
    { name: 'Pengiriman', description: loremIpsum },
    { name: 'Pembayaran', description: loremIpsum },
    { name: 'Pengembalian', description: loremIpsum },
]

export default {
    data() {
        return {
            services
        }
    }
}
</script>