<template>
    <div id="footerbot" class="text-white">
        <div class="container d-flex justify-content-between align-items-center ">
            <div>
                <button>
                    SIGN-UP NOW
                </button>
            </div>
            <div class="d-flex align-items-center">
                <span>
                    FOLLOW US
                </span>

                <ul>
                    <li v-for="(item, index) in followList">
                        <a href="">
                           <img :src="item.img" alt="Icons">
                        </a>
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'footerbot',
        data(){
            return {
                // we create the array of objects for the footerbot to create our CTA 
                followList: [
                    {
                        img: '/img/footer-facebook.png'
                    },
                    {
                        img: '/img/footer-twitter.png'
                    },
                    {
                        img: '/img/footer-youtube.png'
                    },
                    {
                        img: '/img/footer-pinterest.png'
                    },
                    {
                        img: '/img/footer-periscope.png'
                    }
                ]
            }
        }
        
    }
</script>

<style lang="scss" scoped>
@use '../assets/styles/partials/variables' as *;
#footerbot {
    background-color: $backgroundFooterBot;
    padding: 20px;
}
ul {
    list-style-type: none;
    display: flex;
    li {
        padding: 5px;
        img {
            padding-top: 5px;
        }
    }
}
button {
    border: 2px solid $backgroundFooter;
    background: none;
    color: white;
    font-weight: 600;
    padding: 10px;
    margin-top: 5px;
}
span {
    font-weight: 600;
    color: $backgroundFooter;
}


</style>