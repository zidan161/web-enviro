<template>
    <div class="container flex flex-col space-y-16 px-20">
        <h1 class="text-3xl font-extrabold text-gray-900 sm:text-4xl md:text-5xl">
            Jasa Layanan
        </h1>
        <div class="flex flex-col md:flex-row space-x-20">
            <img src="/company.jpg" alt="image company" class="rounded-lg max-w-md">
            <div class="flex flex-col space-y-7">
                <ItemDoc v-for="doc in listDoc" :key="doc.name" :doc="doc"/>
            </div>
        </div>
    </div>
</template>

<script>
const listDoc = [
    {name: 'halo'},
    {name: 'halo'},
    {name: 'halo'},
    {name: 'halo'},
    {name: 'halo'},
    {name: 'halo'},
]

export default {
    data() {
        return {
            listDoc
        }
    },
}
</script>
