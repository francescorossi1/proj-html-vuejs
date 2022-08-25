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

.tc-lime {
  color: $tc-9
}

.tc-white {
  color: $tc-1
}

.lime-button a,
.lime {
  background-image: linear-gradient(to right, #A5E57C, #D2405D)
}

.reverse-lime {
  background-image: linear-gradient(to left, #A5E57C, #D2405D)
}

.black-button a,
.black {
  background-image: linear-gradient(to right, $tc-14, $tc-18)
}
</style>
