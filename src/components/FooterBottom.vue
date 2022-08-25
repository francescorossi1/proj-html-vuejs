<template>
    <div class="container-fluid black py-4">
        <div class="d-flex justify-content-between align-items-center py-3">
            <div class="text-muted">&#169; PHLOX BUSINESS THEME</div>
        <div class="footer-socials">
            <a href="#" v-for="social in footerSocials" :key="social.name" class="me-3 text-muted"><i class="fa-brands"
                    :class="social.icon"></i></a>
        </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'FooterBottom',
    data() {
        return {
            footerSocials: [
                { url: '#', name: 'facebook', icon: 'fa-facebook-f' },
                { url: '#', name: 'twitter', icon: 'fa-twitter' },
                { url: '#', name: 'pinterest', icon: 'fa-pinterest-p' }
            ]
        }
    }
}
</script>

<style>
</style>