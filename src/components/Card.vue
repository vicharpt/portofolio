<template>
    <div class="mb-12 p-4 md:w-1/2 lg:w-1/3">
        <div class="rounded-md shadow-md overflow-hidden">
            <img :src="img.source" :alt="img.alt">
        </div>
        <!-- {{ img.source }} -->
        <h3 class="font-semibold text-xl text-dark mt-5 mb-3">{{ img.title }}</h3>
        <p class="font-medium text-base text-secondary">{{ img.desc }}</p>
    </div>
</template>

<script>
    export default {
        props: {
            img: {
                type: Object,
                required: true
            } 
        }
    }
</script>