<template>
    <div class="jumbotron jumbotron-fluid py-5">
        <div class="container py-5">
            <div class="d-flex">
                <div class="w-50">
                    <h3 class="tc-lime">17 YEARS OF EXPERIENCE</h3>
                    <h1 class="display-1"><strong>We Are a Web Design <span class="tc-lime">Agency</span></strong></h1>
                    <LimeBreak />
                    <p class="pb-3"> Far Far away, behind the word mountains, far From the countries Vokalia and
                        Consonantia, there live
                        the
                        blind texts.
                        Separated they live in Bookmarksgrove right at the coast of the Semantics, a large language
                        ocean.
                        Separated they live in Bookmarksgrove.
                    </p>
                    <BaseButton text='PURCHASE' class="lime-button mb-5" />
                    <div class="d-flex">
                        <span class="" v-for="(link, i) in links" :key="link.name">
                            <a :href="link.url" class="text-black">{{ link.name.toUpperCase() }}</a>
                            <span class="mx-2" v-if="i < (links.length - 1)">-</span>
                        </span>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import LimeBreak from './LimeBreak.vue';
import BaseButton from './BaseButton.vue';


export default {
    name: 'MainJumbotron',
    components: { LimeBreak, BaseButton },
    data() {
        return {
            links: [
                { url: '#', name: 'facebook' },
                { url: '#', name: 'instagram' },
                { url: '#', name: 'youtube' },
                { url: '#', name: 'twitter' }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../assets/sass/vars';

.jumbotron {
    background-image: url('../assets/img/slider-1.png');
    background-repeat: no-repeat;
    background-position: right;
    background-size: 60vw;
    background-color: #F9F9F9;
}
</style>