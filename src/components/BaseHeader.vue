<template>
    <div>
        <div class="bg-header-top py-2">
            <div class="container d-flex justify-content-between">
                <div class="header-numbers">
                    <span class="prefix">(001) </span>
                    <span v-for="item in phone" :key="item.number" class="pe-2"><a href="#">{{item.number}}</a></span>
                </div>
                <div class="header-socials">
                    <a href="#" v-for="social in socials" :key="social.name" class="me-3"><i class="fa-brands" :class="social.icon"></i></a>
                </div>
            </div>
        </div>
        <div class="bg-header-bottom py-4">
            <div class="container d-flex justify-content-between align-items-center">
                <div class="logo"><img src="../assets/img/logo.png" alt="Pilox Logo"></div>
                <ul class="header-menu d-flex my-0">
                    <li v-for="item in menuItems" :key="item.id" class="me-3"><a href="#">{{item.name.toUpperCase()}}</a></li>
                </ul>
                <div class="header-search d-flex">
                    <BaseButton text="PURCHASE" />
                    <a href="#" class="align-middle ms-2"><i class="fa-solid fa-magnifying-glass"></i></a>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import BaseButton from './BaseButton.vue';
export default {
    name: 'BaseHeader',
    data() {
        return {
            phone: [
                { number: 88451234 },
                { number: 88455438 },
            ],
            menuItems: [
                { id: 1, name: 'home' },
                { id: 2, name: 'about' },
                { id: 3, name: 'services' },
                { id: 4, name: 'showcase' },
                { id: 5, name: 'blog' },
                { id: 6, name: 'contacts' }
            ],
            socials: [
                { url: '#', name: 'facebook', icon: 'fa-facebook-f'},
                { url: '#', name: 'twitter', icon: 'fa-twitter'},
                { url: '#', name: 'pinterest', icon: 'fa-pinterest-p'}
            ]
        }
    },
        components: {BaseButton}
}
</script>

<style lang="scss" scoped>
@import '../assets/sass/vars';


.bg-header-top {
    background-color: $bgc-10;
    a, .prefix {
        color: $tc-1;
    }
}

.bg-header-bottom {
    background-color: $bgc-1;
    a {
        color: $tc-15;
        padding-right: 30px;
    }
}
</style>