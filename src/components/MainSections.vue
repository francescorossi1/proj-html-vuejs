<template>
    <div>
        <MainJumbotron />
        <BenefitsSection class="py-lg" />
        <ObjectivesSection />
    </div>
</template>

<script>
import MainJumbotron from './MainJumbotron.vue';
import BenefitsSection from './BenefitsSection.vue';
import ObjectivesSection from './ObjectivesSection.vue';
export default {
    name: 'MainSections',
    components: { MainJumbotron, BenefitsSection, ObjectivesSection }
}
</script>

<style scoped lang="scss">
</style>