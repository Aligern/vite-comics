<template>
    <div>
        <div id="card">
            <img  :src="image" class="w-100 img-fluid " :alt="type">
            <div class="ls-hover">
                <div class="buy">
                    Acquista
                </div>
            </div>
        </div>
        <div id="title">
            <h6>
                {{ title }}
            </h6>
            <span>
                {{ price }}
            </span>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'CardComponent',
        props: [
            'image',
            'type',
            'title',
            'price'
        ]
    }
</script>

<style lang="scss" scoped>
@use '../assets/styles/partials/variables' as *;
#card {
    position: relative;
    &:hover {
        img {
            opacity: 0.3;
        }
        .buy {
        opacity: 1;
    }
    }
    img {
    min-height: 300px;
    margin-bottom: 10px;
    transition: .5s ease;
    backface-visibility: hidden;
}
.ls-hover {
    transition: .5s ease;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    text-align: center;
}
.buy {
    background-color: $backgroundFooter;
    color: white;
    font-size: 16px;
    font-weight: 600;
    padding: 10px 10px;
    border-radius: 15px;
    opacity: 0;
    cursor: pointer;
    transition: .7s ease;
}
}
#title {
    margin-bottom: 50px;
}

</style>