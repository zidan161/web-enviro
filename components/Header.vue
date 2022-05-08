<template>
    <div>
        <!-- create hero using tailwindcss -->
        <div  style="background-image: url(/fotos/foto1.jpeg)" class="h-screen bg-cover">
            <Navbar/>

            <div>
                <div class="flex flex-wrap content-center p-10">
                    <div class="w-full px-4">
                        <h1 class="text-4xl font-extrabold text-white sm:text-5xl md:text-6xl">
                            PT. Tirta Persada Enviro
                        </h1>
                        <p class="text-white text-lg mt-4">
                            Environmental Consultant And Constructions company.
                        </p>
                        <div class="flex space-x-4 mb-6 text-sm font-medium pt-10">
                            <NuxtLink to="/contact">  
                                <button class="px-10 py-3 text-xl font-semibold rounded-full bg-blue-700 hover:bg-blue-800 text-white" type="submit">
                                    Hubungi Kami
                                </button>
                            </NuxtLink>  
                        </div>
                    </div>
                    <!-- <div class="w-full lg:w-6/12 px-4">
                        <img class="h-full w-full object-cover object-center rounded-md" src="/fotos/foto1.jpeg" alt="hero image">
                    </div> -->
                </div>
            </div>
        </div>
    </div>
</template>