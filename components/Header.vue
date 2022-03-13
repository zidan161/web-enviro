<template>
    <div>
        <!-- create hero using tailwindcss -->
        <div>
            <nav class="bg-white shadow">
                <div class="container mx-auto px-6 py-4">
                    <div class="flex items-center justify-between">
                        <div class="flex items-center">
                            <a href="/" class="text-lg font-semibold text-gray-900 no-underline">
                                <img src="https://tailwindcss.com/img/logos/workflow-mark-on-white.svg" alt="Workflow" class="h-8">
                            </a>
                        </div>
                        <div class="flex space-x-5">
                            <a v-for="item in navigation" :key="item.name" :href="item.href" class="font-medium text-gray-500 hover:text-gray-900">{{ item.name }}</a>
                        </div>
                    </div>
                </div>
            </nav>

            <div class="container mx-auto px-4 py-10">
                <div class="flex flex-wrap items-center">
                    <div class="w-full lg:w-6/12 px-4">
                        <h1 class="text-4xl font-extrabold text-gray-900 sm:text-5xl md:text-6xl">
                            Hello World!
                        </h1>
                        <p class="text-gray-600 text-lg mt-4">
                            this is new website hello world
                        </p>
                        <div class="flex space-x-4 mb-6 text-sm font-medium mt-6">
                            <div class="flex-auto flex space-x-4">
                                <button class="h-10 px-6 font-semibold rounded-md bg-black text-white" type="submit">
                                    Buy now
                                </button>
                                <button class="h-10 px-6 font-semibold rounded-md border border-slate-200 text-slate-900" type="button">
                                    Add to bag
                                </button>
                            </div>
                        </div>
                    </div>
                    <div class="w-full lg:w-6/12 px-4">
                        <img class="h-full w-full object-cover object-center rounded-md" src="https://tailwindcss.com/img/card-top.jpg" alt="hero image">
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>

const navigation = [
  { name: 'About', href: '/about' },
  { name: 'Features', href: '#' },
  { name: 'Marketplace', href: '#' },
  { name: 'Company', href: '#' },
]

export default {
    data() {
        return {
            navigation
        }
    }
}
</script>
