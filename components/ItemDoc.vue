<template>
    <div class="flex flex-row space-x-5 content-center">
       <div class="bg-transparent grow-0 lg:bg-blue-400 lg:shadow-md rounded-full p-1">
            <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" viewBox="0 0 20 20" fill="white">
                <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd" />
            </svg>
        </div>
        <p class="text-center text-gray-600">{{ doc.name }}</p>
    </div>
</template>

<script>
export default {
    props: ['doc'],
}
</script>