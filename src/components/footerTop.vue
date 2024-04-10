<template>
    <div class="text-white">
        <ul>
            <li v-for="(item, index) in navFooter" :key="index">
                <img :src="item.img" alt="">
                <a href="item.url">
                    {{ item.text }}
                </a>
            </li>
        </ul>
    </div>
</template>

<script>
    export default {
        name: 'footerTop',
        data() {
            return {
                navFooter: [
                    {
                        img: '/img/buy-comics-digital-comics.png',
                        text: 'Digital Comics',
                        url: '#'
                    },
                    {
                        img: '/img/buy-comics-merchandise.png',
                        text: 'DC Merchandise',
                        url: '#'
                    },
                    {
                        img: '/img/buy-comics-subscriptions.png',
                        text: 'Subscriptions',
                        url: '#'
                    },
                    {
                        img: '/img/buy-comics-shop-locator.png',
                        text: 'Comic Shop Locator',
                        url: '#'
                    },
                    {
                        img: '/img/buy-dc-power-visa.svg',
                        text: 'Dc Power Visa',
                        url: '#'
                    }
                ]
            }
        }
    }
</script>

<style lang="scss" scoped>
ul {
    list-style-type: none;
    display: flex;
    a {
        text-decoration: none;
    }
}
</style>