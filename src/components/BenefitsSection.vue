<template>
    <div class="d-flex align-items-center section-spacing">
        <div class="fb-40 ps-5">
            <h1 class="display-3">
                <strong>We Are Here to Make Your <span class="tc-lime">Website</span> Look More 
                <span class="tc-lime">Elegant</span> And Stylish!</strong>
            </h1>
            <LimeBreak />
            <BaseButton text='VIEW ALL' class="lime-button mb-5" />
        </div>
        <div class="fb-60 row row-cols-2">
            <BaseCard v-for="card in cards" :key="card.id" :card="card" class="col p-3" />

        </div>
    </div>
</template>

<script>
import BaseCard from './BaseCard.vue';
import BaseButton from './BaseButton.vue';
import LimeBreak from './LimeBreak.vue'
export default {
    name: 'BenefitsSection',
    components: { BaseCard, BaseButton, LimeBreak },
    data() {
        return {
            cards: [
                { id: 1, title: 'Speed Optimization', text: 'Far Far away, behind the word mountains, far From the countries Vokalia...', icon: 'fa-solid fa-gauge-simple-high fa-2x' },
                { id: 2, title: 'Cloud Solutions', text: 'Far Far away, behind the word mountains, far From the countries Vokalia...', icon: 'fa-solid fa-cloud fa-2x' },
                { id: 3, title: 'Website Design', text: 'Far Far away, behind the word mountains, far From the countries Vokalia...', icon: 'fa-solid fa-tablet-screen-button fa-2x' },
                { id: 4, title: 'Online Marketing', text: 'Far Far away, behind the word mountains, far From the countries Vokalia...', icon: 'fa-regular fa-clock fa-2x' },
            ]
        }
    }
}
</script>

<style>
</style>