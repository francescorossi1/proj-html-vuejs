<template>
    <div class="d-flex py-3">
        <div class="hr lime sm"></div>
        <div class="hr lime lg"></div>
    </div>
</template>

<script>
export default {
    name: 'LimeBreak'
}
</script>

<style lang="scss" scoped>
.hr {
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