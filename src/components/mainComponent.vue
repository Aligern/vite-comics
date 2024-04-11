<template>
    <div id="main" class="text-white ps-5 pt-3">
        <div id="mainTitle">
            <h5>
           Current Series
            </h5>
        </div>
        
        <div id="cards" class="row" >
            <div id="cardCol" class="col-12 col-md-3" v-for="(item, index) in comics" :key="index">
                <CardComponent :image="item.thumb" :type="item.type" :title="item.series" />
            </div>
        </div>
    </div>
</template>

<script>
import { comics } from '../data/store';
import CardComponent from './CardComponent.vue';
    export default {
        name: 'MainComponent',
        components: {
            CardComponent
        },
        data()  {
            return {
                comics
            }
        }
    }
</script>

<style lang="scss" scoped>
@use '../assets/styles/partials/variables' as *; 
    #mainTitle {
        background-color: $backgroundFooter;
        width: 150px;
        padding: 5px;
        text-align: center;
    }
</style>