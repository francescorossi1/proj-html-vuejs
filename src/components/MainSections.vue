<template>
    <div class="jumbotron">
        <div class="container">
            <h3 class="tc-lime">17 YEARS OF EXPERIENCE</h3>
            <h1 class="display-1">We Are a Web Design <span class="tc-lime">Agency</span></h1>
            <LimeBreak />
            <p> Far Far away, behind the word mountains, far From the countries Vokalia and Consonantia, there live the
                blind texts.
                Separated they rye in Bookmarksgrove right at the coast of the Semantics, a large language ocean.
                Separated they live in Bookmarksgrove.
            </p>
            <BaseButton text='PURCHASE' />
        </div>
    </div>
</template>

<script>
import LimeBreak from './LimeBreak.vue';
import BaseButton from './BaseButton.vue';

export default {
    name: 'MainSections',
    components: { LimeBreak, BaseButton }
}
</script>

<style scoped lang="scss">
.jumbotron {
    background-image: url('../assets/img/slider-1.png');
}
</style>