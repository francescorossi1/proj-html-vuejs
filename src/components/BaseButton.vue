<template>
  <div>
    <a href="#" class="lime tc-white rounded-5">{{text}}</a>
  </div>
</template>

<script>
export default {
    name: 'BaseButton',
    props: {text: String}
}
</script>

<style scoped lang="scss">
@import '../assets/sass/vars';
    a{
        padding: 12px 30px;
        font-size: 10px;
        color: $tc-1;
    }
</style>