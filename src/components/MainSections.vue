<template>
    <div class="container">
        <h3 class="tc-lime">17 YEARS OF EXPERIENCE</h3>
        <h1 class="display-1">We Are a Web Design <span class="tc-lime">Agency</span></h1>
        <LimeBreak />
    </div>
</template>

<script>
import LimeBreak from './LimeBreak.vue'
export default {
    name: 'MainSections',
    components: {LimeBreak}
}
</script>

<style scoped lang="scss">
div {
    background-image: url('../assets/img/slider-1.png');
    height: 700px;
}
</style>