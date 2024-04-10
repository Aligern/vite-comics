<template>
<header class=" pt-3 pb-3 ps-5">
    <div class="d-flex justify-content-evenly align-items-center">
        <div>
            <img :src="logoNavbar" alt="Logo">
        </div>
        <div>
            <ul>
                <li v-for="(item, index) in navBar">
                   <a href="item.url">{{ item.name }}</a> 
                </li>
            </ul>
        </div>
    </div>
</header>
</template>

<script>
    export default {
        name: 'headerComponent',
        data() {
            return {
                logoNavbar:'./img/dc-logo.png',
                navBar: [
                    {
                        name: 'CHARACTERS',
                        url: '#',
                    },
                    {
                        name: 'COMICS',
                        url: '#',
                    },
                    {
                        name: 'MOVIES',
                        url: '#',
                    },
                    {
                        name: 'TV',
                        url: '#',
                    },
                    {
                        name: 'GAMES',
                        url: '#',
                    },
                    {
                        name: 'COLLECTIBLES',
                        url: '#',
                    },
                    {
                        name: 'VIDEOS',
                        url: '#',
                    },
                    {
                        name: 'FANS',
                        url: '#',
                    },
                    {
                        name: 'NEWS',
                        url: '#',
                    },
                    {
                        name: 'SHOP',
                        url: '#',
                    }
                ]
            }
        }
    }
</script>

<style lang="scss" scoped>
    $backgroundNav: #FFFFFF;
header {
    background-color: $backgroundNav;
        ul{
        list-style-type: none;
        display: flex;
}
        li {
            padding: 6px;
            a{
                text-decoration: none;
                color: black;
            }
}
}
</style>