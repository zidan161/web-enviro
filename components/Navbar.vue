<template>
    <nav>
        <div class="mx-auto px-10 py-7 bg-white">
            <div class="flex items-center justify-between">
                <div class="flex items-center">
                    <NuxtLink to="/" class="text-lg font-semibold text-white no-underline">
                        <img src="/logo_tirta.png" alt="Workflow" class="h-10">
                    </NuxtLink>
                </div>
                <div class="flex space-x-5">
                    <NuxtLink v-for="item in navigation" :key="item.name" :to="item.href" class="font-medium text-gray-700 hover:text-gray-400">{{ item.name }}</NuxtLink>
                </div>
            </div>
        </div>
    </nav>
</template>

<script>
const navigation = [
  { name: 'About', href: '/about' },
  { name: 'Gallery', href: '/gallery' },
  { name: 'Clients', href: '/clients' },
  { name: 'Contact Us', href: '/contact' },
]

export default {
    data() {
        return {
            navigation
        }
    }
}
</script>
