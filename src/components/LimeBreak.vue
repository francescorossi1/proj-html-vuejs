<template>
    <div class="d-flex py-5">
        <div class="hr sm"></div>
        <div class="hr lg"></div>
    </div>
</template>

<script>
export default {
    name: 'LimeBreak'
}
</script>

<style lang="scss" scoped>
.hr {
    background-image: linear-gradient(to right, #A5E57C, #00D9A6);
    height: 5px;
    border-radius: 3px;
    margin-left: 5px;

    &.sm {
        width: 8px;
    }

    &.lg {
        width: 48px;
    }
}
</style>