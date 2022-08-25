<template>
    <div class="col">
        <img :src="require(`../assets/img/${sample.src}`)" :alt="sample.title" class="img-fluid rounded-3">
        <div class="content">
            <h6>{{sample.title}}</h6>
            <span>{{sample.type.toUpperCase()}}</span>
        </div>
    </div>
</template>

<script>
export default {
    name: 'SamplesCard',
    props: {sample: Object}
}
</script>

<style lang="scss" scoped>
.col {
    transition: scale 0.3s linear, transform 0.3s linear;
}

.col .content {
    display: none;
    position: absolute;
    bottom: 10%;
    left: 10%;
}

.col:hover {
    scale: 1.1;
    transform: translateY(-5%);
}

.col:hover .content {
    display: block;
    color: white;
}

.col:hover::before {
    content: "";
    position: absolute;
    bottom: 0;
    top: 0;
    right: 0;
    left: 0;
    background-image: linear-gradient(to top right, rgb(165, 229, 124), rgba(210, 64, 93, 0.6));
    border-radius: 8px;
}
</style>