<script setup>
import Layout from '@/Layouts/Layout.vue';
import SlideBanner from '@/Components/SlideBanner.vue';
import SlideFormacoes from '@/Components/SlideFormacoes.vue';
import InfoCards from '@/Components/InfoCards.vue';

defineProps({
    canLogin: Boolean,
    canRegister: Boolean,
    laravelVersion: {
        type: String,
        required: true,
    },
    phpVersion: {
        type: String,
        required: true,
    },
});



</script>

<template>
    <Layout>
        <SlideBanner />
        <div class="bg-white px-12"> 
            <div class="flex text-center w-full justify-center items-center p-12 flex-col">
            <h3 class="md:text-2xl text-xl">ABRATEF</h3>
            <p class="lg:w-1/2 md:w-full w-full md:normal-case text-justify md:text-center"> é uma Organização da Sociedade Civil (OSC), fundada em 1994, sem fins lucrativos e econômicos, de interesse público, apartidária e de âmbito nacional.</p>
            </div>
            <div class="grid grid-cols-1 gap-4 lg:grid-cols-3 lg:gap-8">
                <div class="">
                    <InfoCards title="O que é Terapia Familiar ?"
                        textInfo=" Lorem ipsum dolor sit amet consectetur adipisicing elit. Cupiditate, praesentium voluptatem omnis atque culpa repellendus."
                        link="/"
                        linkImg="https://res.cloudinary.com/dtf70ty3b/image/upload/v1710116821/terapia/info1.jpg" />
                </div>
                <div class="">
                    <InfoCards title="Seja um Associado ABRATEF"
                        textInfo=" Lorem ipsum dolor sit amet consectetur adipisicing elit. Cupiditate, praesentium voluptatem omnis atque culpa repellendus."
                        link="/"
                        linkImg="https://res.cloudinary.com/dtf70ty3b/image/upload/v1710116821/terapia/info2.jpg" />
                </div>
                <div class="">
                    <InfoCards title="Formação em Terapia Familiar"
                        textInfo=" Lorem ipsum dolor sit amet consectetur adipisicing elit. Cupiditate, praesentium voluptatem omnis atque culpa repellendus."
                        link="/"
                        linkImg="https://res.cloudinary.com/dtf70ty3b/image/upload/v1710116821/terapia/info3.jpg" />
                </div>
            </div>
            <div class="py-12">
               <div class="">
                <h3 class="w-2/3 border-b-2 border-solid border-black text-2xl ">Principais Formações</h3>
               </div>
               <SlideFormacoes />
            </div>
        </div>
    </Layout>
</template>import SlideFormacoesVue from '@/Components/SlideFormacoes.vue';

