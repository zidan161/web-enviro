<template>
    <div class="flex flex-col space-y-10 px-14">
        <h2 class="text-4xl text-center font-extrabold text-gray-900 mb-7 lg:text-6xl">
            Klien Kami
        </h2>
        <div class="grid grid-cols-2 gap-4 md:grid-cols-5">
            <ItemClient v-for="item in clients" :key="item.id" :image="item.image" :name="item.name"/>
        </div>
    </div>
</template>

<script>
const clients = [
    {id: 1, name: 'Dana Paint', image: '/dana_paint.png'},
    {id: 2, name: 'RS Sido Waras', image: '/sido_waras.png'},
    {id: 3, name: 'RSU Jasem', image: '/logo_rsu_jasem.png'},
    {id: 4, name: 'Ibis Hotel', image: '/hotel_ibis.png'},
    {id: 5, name: 'Intipack', image: '/intipack_logo.png'},
    {id: 6, name: 'Selecta', image: '/selecta_logo.png'},
    {id: 7, name: 'RS Sakinah', image: '/sakinah.png'},
    {id: 8, name: 'Fortuna Lab', image: '/fortuna_lab.png'},
    {id: 9, name: 'Hotel Aston', image: '/aston_logo.png'},
    {id: 10, name: 'RS Metro', image: '/metro.png'},
]

export default {
    data() {
        return {
            clients
        }
    },
}
</script>