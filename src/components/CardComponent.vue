<template>
    <div>
        <div id="card">
            <img  :src="image" :alt="type">
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
    width: 150px;
    height: 200px;
    margin-bottom: 10px;
}
}

#title {
    margin-bottom: 50px;
}

</style>