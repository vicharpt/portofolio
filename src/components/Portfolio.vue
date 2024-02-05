<template>
    <section id="portfolio" class="pt-24 pb-16 bg-slate-100">
        <div class="container">
            <div class="w-full px-4">
                <div class="max-w-xl mx-auto text-center mb-16">
                    <h4 class="font-semibold text-md text-primary mb-2">Portfolio</h4>
                    <h2 class="font-bold text-dark text-2xl mb-4">Project Terbaru</h2>
                    <p class="font-medium text-medium text-secondary">Lorem ipsum dolor sit amet consectetur adipisicing elit. Natus laboriosam quia, accusamus tenetur perspiciatis maiores.</p>
                </div>
            </div>

            <div class="w-full px-4 flex flex-wrap">
                <Card  :img="img" v-for="img in images"/>
            </div>
        </div>
    </section>
</template>

<script>
    import Card from './Card.vue';

    export default {
        components: {
            Card
        },
        data() {
            return {
                images: [
                    {
                        source: 'src/assets/foto.png',
                        alt: 'title 1',
                        title: 'Titile 1',
                        desc: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Doloribus ipsum in perspiciatis?'
                    },
                    {
                        source: 'src/assets/foto.png',
                        alt: 'title 2',
                        title: 'Titile 2',
                        desc: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Doloribus ipsum in perspiciatis?'
                    },
                    {
                        source: 'src/assets/foto.png',
                        alt: 'title 3',
                        title: 'Titile 3',
                        desc: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Doloribus ipsum in perspiciatis?'
                    },
                    {
                        source: 'src/assets/foto.png',
                        alt: 'title 4',
                        title: 'Titile 4',
                        desc: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Doloribus ipsum in perspiciatis?'
                    }
                ]
            }
        }
    }
</script>