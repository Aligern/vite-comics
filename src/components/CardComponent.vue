<template>
    <div>
        <div class="card">
            <img :src="image" :alt="type">
        </div>
        <div>
            <h4>{{ title }}</h4>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'CardComponent',
        props: [
            'image',
            'type',
            'title'
        ]
    }
</script>

<style lang="scss" scoped>

</style>