<template>
    <div>
        <div class="base-card p-5 rounded-5 h-100">
            <div class="card-content">
                <i :class="card.icon" class="py-2"></i>
                <h2 class="py-2">{{ card.title }}</h2>
                <p class="py-2">{{ card.text }}</p>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'BaseCard',
    props: { card: Object }
}
</script>
<style lang="scss" scoped>
@import '../assets/sass/vars.scss';
    .base-card{
        box-shadow: 0px 0px 20px 10px $bgc-4;
        transition: color 0.5s linear, background-image 0.5s linear;
    &:hover{
        background-image: linear-gradient(to bottom left, #A5E57C, #D2405D);
        color: $tc-1
        }
    }
</style>