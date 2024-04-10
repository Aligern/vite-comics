<template>
<header>
    <div class="d-flex justify-content-between">
        <div>
            <img src="/img/dc-logo.png" alt="Logo">
        </div>
        <div>
            <ul>
                <li>
                    <a href="#">
                        Characters
                    </a>
                </li>
                <li>
                    <a href="#">
                        Comics
                    </a>
                </li>
                <li>
                    <a href="#">
                        Movies
                    </a>
                </li>
                <li>
                    <a href="#">
                        TV
                    </a>
                </li>
                <li>
                    <a href="#">
                        Games
                    </a>
                </li>
                <li>
                    <a href="#">
                        Collectibles
                    </a>
                </li>
                <li>
                    <a href="#">
                        Videos
                    </a>
                </li>
                <li>
                    <a href="#">
                        Fans
                    </a>
                </li>
                <li>
                    <a href="#">
                        News
                    </a>
                </li>
                <li>
                    <a href="#">
                        Shop
                    </a>
                </li>
            </ul>
        </div>
    </div>
</header>
</template>

<script>
    export default {
        name: 'headerComponent',
    }
</script>

<style lang="scss" scoped>
    ul{
    list-style-type: none;
    display: flex;
        li {
            padding: 6px;
            
}
}

</style>