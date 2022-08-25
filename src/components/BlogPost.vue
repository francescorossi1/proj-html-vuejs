<template>
    <div>
        <div class="card-img">
            <div>
                <img :src="require(`../assets/img/${post.src}`)" :alt=post.title class="img-fluid rounded-3">
            </div>
        </div>
        <div class="card-txt text-start">
            <span class="text-muted">{{ post.date }} by {{ post.author }}</span>
            <h4>{{ post.title }}</h4>
        </div>
    </div>
</template>

<script>
export default {
    name: 'BlogPost',
    props: { post: Object }
}
</script>

<style lang="scss" scoped>
@import '../assets/sass/vars.scss';

.card-img {
    box-shadow: 0px 0px 20px 10px $bgc-5;
}

.card-txt {
    min-height: 190px;
    padding: 50px 30px;
    margin: 0 30px;
    border-radius: 15px;
    background-color: $bgc-1;
    transform: translateY(-50%);

    h4::before {
        content: "\25CF";
        color: $tc-9
    }
}
</style>