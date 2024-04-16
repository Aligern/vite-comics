<template>
    <FooterTop />
    <FooterMid />
    <Footerbot />
</template>

<script>
// we take the footerTop, footerMid and footerbot components
import FooterTop from './FooterTop.vue';
import FooterMid from './FooterMid.vue';
import Footerbot from './FooterBot.vue';
    export default {
        name: 'FooterComponent',
        components: {
            FooterTop,
            FooterMid,
            Footerbot
        },  
    }
</script>

<style lang="scss" scoped>

</style>