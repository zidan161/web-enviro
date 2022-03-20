<template>
    <div class="shadow-md rounded-xl p-4 max-w-sm">
        <div class="flex flex-col items-center">
            <h2 class="font-extrabold text-gray-900">{{ service.name }}</h2>
            <p class="text-center">{{ service.description }}</p>
        </div>
    </div>
</template>

<script>
export default {
    props: ['service'],
}
</script>