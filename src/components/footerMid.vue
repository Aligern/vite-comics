<template>
    <div id="footerMid" class="container text-white">
       <div> 
        <ul  v-for="(item, index) in footerList" :key="index">
            {{ item.title }}
            <li v-for="(item, index) in item.list" :key="index">
                {{ item.list }}
            </li>
        </ul>
       </div>

       <div>
        right
       </div>
    </div>
</template>

<script>
    export default {
        name: 'footerMid',
        data() {
            return {
                footerList: [
                    {
                        title: 'DC COMICS',
                        list: [
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
                        list: [
                            'Shop DC',
                            'Shop DC Collectibles'
                        ]
                    },
                    {
                        title: 'DC',
                        list: [
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
                        list: [
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
#footerMid {
    height: 200px;
    display: flex;
    justify-content: space-between;
}

</style>