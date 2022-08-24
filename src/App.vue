<template>
  <div>
    <BaseHeader />
    <MainSections />
  </div>
</template>

<script>
import BaseHeader from './components/BaseHeader.vue';
import MainSections from './components/MainSections.vue';


export default {
  name: 'App',
  components: {
    BaseHeader,
    MainSections
}
}
</script>

<style lang="scss">
@import './assets/sass/style.scss';
.tc-lime { color: $tc-9 }
</style>
