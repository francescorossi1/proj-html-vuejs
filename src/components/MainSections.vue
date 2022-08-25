<template>
    <div>
        <MainJumbotron />
        <BenefitsSection class="py-lg" />
        <ObjectivesSection />
        <SamplesSection class="py-lg" />
        <QuotesSection />
        <BlogSection />
    </div>
</template>

<script>
import MainJumbotron from './MainJumbotron.vue';
import BenefitsSection from './BenefitsSection.vue';
import ObjectivesSection from './ObjectivesSection.vue';
import SamplesSection from './SamplesSection.vue';
import QuotesSection from './QuotesSection.vue';
import BlogSection from './BlogSection.vue';
export default {
    name: 'MainSections',
    components: { MainJumbotron, BenefitsSection, ObjectivesSection, SamplesSection, QuotesSection, BlogSection }
}
</script>

<style scoped lang="scss">
</style>