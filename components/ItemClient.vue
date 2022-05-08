<template>
    <div class="flex p-5 rounded-md shadow-md justify-center hover:shadow-lg">
        <img :src="'/clients'+this.image" :alt="this.name" :name="this.name" class="object-contain max-h-20">
    </div>
</template>

<script>
export default {
    props: ['image', 'name'],
}
</script>