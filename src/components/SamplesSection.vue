<template>
    <div>
        <div class="container-fluid d-flex align-items-end pb-5">
            <div class="w-50">
                <LimeBreak />
                <h2 class="display-3">
                    <strong>Our recent <span class="tc-lime">Web Designs</span>
                        & Some Examples of Past <span class="tc-lime">Projects</span></strong>
                </h2>
                <LimeBreak />
            </div>
            <div class="w-50">
                <p class="pb-5">
                    Far Far away, behind the word mountains, far From the countries Vokalia and
                    Consonantia, there live the blind texts.
                    Separated they live in Bookmarksgrove right at the coast of the Semantics, a large language ocean.
                    Separated they live in Bookmarksgrove.
                </p>
            </div>
        </div>
        <div class="gallery">
            <div class="row row-cols-4 gx-1">
                <SamplesCard v-for="sample in samples" :key="sample.id" :sample="sample" />
            </div>
        </div>
    </div>
</template>

<script>
import LimeBreak from './LimeBreak.vue';
import SamplesCard from './SamplesCard.vue'
export default {
    name: 'SamplesSection',
    components: { LimeBreak, SamplesCard },
    data() {
        return {
            samples: [
                { id: 1, src: 'gallery-1.jpg', title: 'A Basket of Flowers', type: 'Design' },
                { id: 2, src: 'gallery-2.jpg', title: 'A Famous Ferris Wheel', type: 'Marketing' },
                { id: 3, src: 'gallery-3.jpg', title: 'A Renowned Brand of Shoes', type: 'Marketing' },
                { id: 4, src: 'gallery-4.jpg', title: 'An Office', type: 'Recruiting' },
                { id: 5, src: 'gallery-5.jpg', title: 'Paper Boats', type: 'Art' },
                { id: 6, src: 'gallery-6.jpg', title: 'Sofa under a light', type: 'Art' },
                { id: 7, src: 'gallery-7.jpg', title: 'Air Balloons', type: 'Tourism' },
                { id: 8, src: 'gallery-8.jpg', title: 'Sliced Orange', type: 'Design' },
            ]
        }
    }
}
</script>