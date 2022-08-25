<template>
  <div class="footer-top py-5">
            <div class="row align-items-center">
                <div class="col-3">
                    <div class="p-2">
                        <img src="../assets/img/logo.png" alt="logo">
                        <p>
                            While the lovely valley teems with vapour around me, and the meridian sun strikes the upper
                            surface of the impenetrable Foliage of my trees.
                            While the lovely valley teems with vapour around me.
                        </p>
                    </div>
                </div>
                <div class="col-3">
                    <div class="p-2">
                        <h3>QUICK LINKS</h3>
                        <LimeBreak />
                        <ul>
                            <li v-for="(link, i) in footerLinks" :key="i"><a href="#"
                                    class="text-black">{{ link.name }}</a></li>
                        </ul>
                    </div>
                </div>
                <div class="col-3">
                    <div class="p-2">
                        <h3>CONTACT</h3>
                        <LimeBreak />
                        <ul>
                            <li class="py-2">{{ contact.address }}</li>
                            <li class="py-2">{{ contact.email }}</li>
                            <li>{{ contact.number }}</li>
                        </ul>
                    </div>
                </div>
                <div class="col-3">
                    <div class="p-2">
                        <h3>LOCATION ON MAP</h3>
                        <LimeBreak />
                        <iframe
                            src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3348.1733914602237!2d-97.07354588495335!3d32.94643128263529!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x864c2b4000000001%3A0xffb9331da6815400!2sPhlox%20Agency!5e0!3m2!1sit!2sit!4v1661442103984!5m2!1sit!2sit"
                            width="100%" height="150" style="border:0;" loading="lazy"
                            referrerpolicy="no-referrer-when-downgrade"></iframe>
                    </div>
                </div>
            </div>
        </div>
</template>

<script>
import LimeBreak from './LimeBreak.vue';
export default {
    name: 'FooterTop',
    components: { LimeBreak },
    data() {
        return {
            footerLinks: [
                { name: 'Careers', url: '#' },
                { name: 'News', url: '#' },
                { name: 'Terms of use', url: '#' },
                { name: 'Privacy Projects', url: '#' },
                { name: 'About', url: '#' },
                { name: 'Contacts', url: '#' },
            ],
            contact: {
                address: 'Patricia C. Amedee 4401 Waldeck Street Grapevine Nashville, TX 76051',
                email: 'info@yourdomain.com',
                number: '+99 (0) 101 0000 888'
            }
        }
    }
}
</script>

<style>

</style>