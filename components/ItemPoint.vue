<template>
    <div class="group flex justify-center bg-white shadow-lg rounded-xl border border-blue-200 hover:bg-blue-200 z-10">
        <h3 class="text-lg text-center font-semibold text-blue-500 p-4 group-hover:text-white">
            {{ service }}
        </h3>
    </div>
</template>

<script>
export default {
    props: ['service'],
}
</script>