<template>
    <div class="bg-gray pb-5">
        <div class="container-fluid pt-2">
            <div class="row row-cols-2 pb-5">
                <div>
                    <NewProjectCard class="rounded-3 black" title="Are you ready?" text="Start a New Project"
                        card-type="form" />
                </div>
                <div>
                    <NewProjectCard class="rounded-3 reverse-lime" title="What are you waiting for?"
                        text="Lets Talk About Work" card-type="button" />
                </div>
            </div>
        </div>
        <div class="clients container-fluid py-5">
            <div class="row row-cols-6">
                <div class="text-muted col" v-for="client in clients" :key="client.id">
                    <img :src="require(`../assets/img/${client.src}`)" :alt="client.name">
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import NewProjectCard from './NewProjectCard.vue';
export default {
    name: "NewProjectSection",
    components: { NewProjectCard },
    data() {
        return {
            clients: [
                { id: 1, src: 'client-1.png', name: 'avantgarde' },
                { id: 2, src: 'client-2.png', name: 'fastlane' },
                { id: 3, src: 'client-3.png', name: 'ron jones' },
                { id: 4, src: 'client-4.png', name: 'chippy\'s' },
                { id: 5, src: 'client-5.png', name: 'bullseye' },
                { id: 6, src: 'client-6.png', name: 'mighty furnitures' },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../assets/sass/vars';

.bg-gray {
    background-color: $bgc-4;
}

.text-muted.col {
    text-align: center;
    line-height: 68px;
}
</style>