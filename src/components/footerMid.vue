<template>
    <div id="footerMid" >
       <div class="container d-flex justify-content-center"> 
        <div id="left" class="text-white d-flex">
            <!-- we print the title and the list -->
            <ul  v-for="(item, index) in footerList" :key="index">
            {{ item.title }}
            <li v-for="(itemlist, i) in item.link" :key="i">
               <a href="">
                {{ itemlist }}
               </a>
            </li>
        </ul>
       </div>
       <div id="right">
       </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'FooterMid',
        data() {
            return {
                // here we create the array of objects for the footerMid to create our menu
                footerList: [
                    {
                        title: 'DC COMICS',
                        link: [
                            'Characters',
                            'Comics',
                            'Movies',
                            'TV',
                            'Games',
                            'Videos',
                            'News'
                        ]
                    },
                    {
                        title: 'SHOP',
                        link: [
                            'Shop DC',
                            'Shop DC Collectibles'
                        ]
                    },
                    {
                        title: 'DC',
                        link: [
                            'Terms Of Use',
                            'Privacy policy (New)',
                            'Ad Choices',
                            'Advertising',
                            'Jobs',
                            'Subscriptions',
                            'Talent Workshops',
                            'CPSC Certificates',
                            'Ratings',
                            'Shop Help',
                            'Contact Us'
                        ]
                    },
                    {
                        title: 'SITES',
                        link: [
                            'DC',
                            'MAD Magazine',
                            'DC Kids',
                            'DC Universe',
                            'DC Power Visa'
                        ]
                    }
                ]
            }
        }
    }
</script>

<style lang="scss" scoped>
@use '../assets/styles/partials/variables' as *;
#footerMid {
    background-image: url('./img/footer-bg.jpg');
    background-size: cover;
    ul {
        list-style-type: none;
        li {
            a {
                text-decoration: none;
                color: rgb(136, 135, 135);
                font-weight: 600;
            }
        }
    }
    #left {
        padding-top: 20px;
        width: 50%;
    }
    #right {
        background-image: url('./img/dc-logo-bg.png');
        width: 50%;
        background-position: right center;
        background-repeat: no-repeat;
        background-size: 70%;
    }
}
</style>