<template>
    <div class="container-fluid">
        <FooterTop />
        <FooterBottom />
    </div>
</template>

<script>
import FooterTop from "./FooterTop.vue";
import FooterBottom from "./FooterBottom.vue";

export default {
    name: "MainFooter",
    components: { FooterTop, FooterBottom },
}
</script>

<style>
.footer-top ul {
    padding: 0
}
</style>