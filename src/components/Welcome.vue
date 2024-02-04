<template>
    <section id="home" class="pt-36 md:pt-24">
        <div class="container">
            <div class="flex flex-wrap">
                <div class="max-w-full self-center px-4 md:w-1/2">
                    <h1 class="text-base font-semibold text-primary md:text-xl mb-1">Hallo Semua 👋, saya <span class="block font-bold text-dark text-4xl mt-1 lg:text-5xl">Indra Saputra</span></h1>
                    <h2 class="font-medium text-secondary text-lg mb-5 lg:text-xl">Web Developer</h2>
                    <p class="font-medium text-secondary mb-10 leading-relaxed">Saya sedang belajar menjadi seorang <span class="text-dark">web developer</span></p>
                    <!-- <p class="font-medium text-secondary leading-relaxed mb-10">Lorem ipsum dolor sit amet consectetur adipisicing elit. Laborum, temporibus velit! Voluptatibus distinctio, provident cupiditate repudiandae facilis impedit iusto quos.</p> -->

                    <a href="" class="text-base font-semibold text-white bg-primary py-3 px-8 rounded-full hover:shadow-lg hover:opacity-80 transition duration-300 ease-in-out">Hubungi saya</a>
                </div>
                <div class="max-w-full self-end px-4 md:w-1/2 overflow-hidden md:overflow-visible">
                    <div class="relative mt-10 lg:mt-0 lg:right-0 text-primary">
                        <img :src="foto" alt="Indra Saputra" class="max-w-full mx-auto" />
                        <span class="absolute bottom-4 -z-10 left-1/2 -translate-x-[60%] md:-translate-x-1/2 md:scale-125 w-full">
                            <svg width="390" height="390" viewBox="0 0 200 200" xmlns="http://www.w3.org/2000/svg">
                                <path fill="currentColor" d="M48.6,-56.9C60.2,-48.2,64.9,-30.3,67.3,-12.5C69.7,5.3,69.8,22.8,63,38C56.2,53.2,42.5,66.1,26.9,70.2C11.3,74.3,-6.2,69.7,-20.4,62C-34.7,54.3,-45.7,43.5,-55.2,30.3C-64.8,17,-72.9,1.4,-71.6,-13.7C-70.2,-28.9,-59.5,-43.5,-46,-51.8C-32.5,-60.1,-16.2,-62.1,1.1,-63.5C18.5,-64.8,37,-65.5,48.6,-56.9Z" transform="translate(100 100)" />
                            </svg>
                        </span>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
    import foto from '../assets/foto.png';
    export default {
        data() {
            return {
                foto: foto
            }
        }
    }
</script>