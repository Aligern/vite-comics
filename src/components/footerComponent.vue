<template>
    <footerTop />
    <footerMid />
    <footerbot />
</template>

<script>
import footerTop from './footerTop.vue';
import footerMid from './footerMid.vue';
import footerbot from './footerbot.vue';
    export default {
        name: 'footerComponent',
        components: {
            footerTop,
            footerMid,
            footerbot
        },  
    }
</script>

<style lang="scss" scoped>

</style>