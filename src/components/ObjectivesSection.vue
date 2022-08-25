<template>
    <div class="d-flex row g-0 align-items-center py-5">
        <div class="col-5">
            <div class="img-bg rounded-5">
                <img src="../assets/img/objectives-1.jpg" alt="Business Woman" class="img-fluid rounded-4">
            </div>
        </div>
        <div class="col-5 offset-1 p-5">
            <h1 class="display-3">
                <strong>learn more about our <span class="tc-lime">missions</span></strong>
            </h1>
            <LimeBreak />
            <p class="pb-3">
                Far Far away, behind the word mountains, far From the countries Vokalia and
                Consonantia, there live the blind texts.
                Separated they live in Bookmarksgrove right at the coast of the Semantics, a large language ocean.
                Separated they live in Bookmarksgrove.
            </p>
            <BaseButton text='READ MORE' class="lime-button mb-5" />
        </div>
    </div>
</template>

<script>
import LimeBreak from './LimeBreak.vue';
import BaseButton from './BaseButton.vue';
export default {
    name: 'ObjectivesSection',
    components: { LimeBreak, BaseButton }
}
</script>

<style lang="scss">
@import '../assets/sass/vars.scss';

.img-bg {
    background-image: linear-gradient(to top right, #A5E57C, #D2405D), url('../assets/img/objectives-2.jpg');

    img {
        transform: translate(10%, 10%);
        box-shadow: 0px 0px 20px 0px $tc-10;
    }
}
</style>