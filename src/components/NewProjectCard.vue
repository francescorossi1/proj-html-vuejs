<template>
    <div>
        <div class="text-center project-card rounded-3 py-5">
            <div class="py-4">
                <span class="text-muted">{{ title }}</span>
                <h4 class="text-white">{{ text }}</h4>
            </div>
            <div v-if="cardType === 'form'" class="py-2">
                <div class="pill-form black d-flex justify-content-between">
                    <input type="text" placeholder="Enter your email address" class="border-0 flex-grow-1">
                    <a href="#" class="text-white-50">Submit</a>
                </div>
            </div>
            <div v-if="cardType === 'button'" class="py-4">
                <BaseButton class="black-button justify-content-center" text="START NOW" />
            </div>
        </div>
    </div>
</template>

<script>
import BaseButton from './BaseButton.vue';
export default {
    name: 'NewProjectCard',
    props: { text: String, title: String, cardType: String },
    components: { BaseButton }
}
</script>

<style lang="scss">
@import '../assets/sass/vars';

.project-card {
    box-shadow: 0px 0px 10px 10px $bgc-5;

    .pill-form {
        background-image: linear-gradient(to right, #4A4A4A, #383838);
        max-width: 70%;
        margin: 0 auto;
        padding: 15px 10px;
        border-radius: 50px;

        input,
        a {
            background-color: transparent;
            border: 0;
        }

    }
}
</style>