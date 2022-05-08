<template>
    <div class="flex flex-row justify-center space-x-20 p-10 bg-gray-800">
        <img src="/logo_tirta.png" alt="Workflow" class="h-10">
        <div>
            <p class="text-white">
                Copyright {{ date }} © Tirta Persada Enviro
            </p>
        </div>
    </div>
</template>

<script>

var date = new Date().getFullYear()

export default {
    data() {
        return {
            date
        }
    },
}
</script>