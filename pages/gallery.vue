<template>
    <div>
        <Navbar/>
        <h1 class="text-4xl text-center p-20 font-extrabold text-gray-900 sm:text-4xl md:text-6xl">
            Gallery
        </h1>
        <img src="/fotos/foto1.jpeg" alt="" class="px-20">
        <div class="grid grid-cols-3 gap-10 p-20">
            <img src="/fotos/foto2.jpeg" alt="">
            <img src="/fotos/foto3.jpeg" alt="">
            <img src="/fotos/foto4.jpeg" alt="">
            <video width="320" height="240" controls>
                <source src="/fotos/video1.mp4" type="video/mp4">
                Your browser does not support the video tag.
            </video>
            <video width="320" height="240" controls>
                <source src="/fotos/video2.mp4" type="video/mp4">
                Your browser does not support the video tag.
            </video>
            <video width="320" height="240" controls>
                <source src="/fotos/video3.mp4" type="video/mp4">
                Your browser does not support the video tag.
            </video>
        </div>
    </div>
</template>