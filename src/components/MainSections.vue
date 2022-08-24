<template>
    <div>
        <MainJumbotron />
        <BenefitsSection class="py-lg"/>
    </div>
</template>

<script>
import MainJumbotron from './MainJumbotron.vue';
import BenefitsSection from './BenefitsSection.vue';
export default {
    name: 'MainSections',
    components: { MainJumbotron, BenefitsSection }
}
</script>

<style scoped lang="scss">
</style>