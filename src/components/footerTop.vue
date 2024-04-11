<template>
    <div id="footerTop" class="text-white">
        <div class="container">
            <div id="box" v-for="(item, index) in navFooter" :key="index">
                <img :src="item.img" alt="Logos">
                <a href="item.url">
                    {{ item.text }}
                </a>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'FooterTop',
        data() {
            return {
                // here we create the array of objects for the footerTop to create our menu
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
@use '../assets/styles/partials/variables' as *;
#footerTop {
    background-color: $backgroundFooter;
    display: flex;
    height: 150px;
    div {
    list-style-type: none;
    display: flex;
    justify-content: space-between;
    #box {
        align-items: center;
        img {
            width: 55px;
            height: 58px;
            display: block;
            padding: 6px;
        }
        a {
        color: white;
        text-decoration: none;
        font-weight: 600;
    }
    }
}
}
</style>