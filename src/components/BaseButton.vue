<template>
    <div>
        <a href="#" class="rounded-5">{{ text }}</a>
    </div>
</template>

<script>
export default {
    name: 'BaseButton',
    props: { text: String }
}
</script>

<style scoped lang="scss">
@import '../assets/sass/vars';

a {
    padding: 15px 35px;
    font-size: 12px;
}

a,
a:hover {
    color: $tc-1;
}
</style>