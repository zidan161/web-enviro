<template>
    <div class="flex flex-row space-x-20">
        <p class="font-semibold">
            {{ this.data.name }}
        </p>
        <p class="">
            {{ this.data.desc }}
        </p>
    </div>
</template>

<script>
export default {
    props: ['data'],
}
</script>