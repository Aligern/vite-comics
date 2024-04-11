<template>
    <div>
        <div id="card">
            <img  :src="image" class="w-100 img-fluid " :alt="type">
        </div>
        <div id="title">
            <h6>
                {{ title }}
            </h6>
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
        ]
    }
</script>

<style lang="scss" scoped>
#card {
    img {
    min-height: 300px;
    margin-bottom: 10px;
}
}

#title {
    margin-bottom: 50px;
}

</style>