<template>
    <div id="main">
        <div id="jumbotron">
        </div>
        <div class="container">
            <div id="mainTitle">
                <h5>
               Current Series
                </h5>
            </div>
            <div id="cards" class="row m-auto text-light" >
                <div id="cardCol" class="col-12 col-md-3 col-lg-2" v-for="(item, index) in comics" :key="index">
                    <CardComponent :image="item.thumb" :type="item.type" :title="item.series" :price="item.price" />
                </div>
            </div>
            <div id="button" class="d-flex justify-content-center">
                <button>
                    Load More
                </button>
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
        width: 200px;
        padding: 5px;
        text-align: center;
        transform: translateY(-50%);
        color: white;
    }
    #jumbotron {
        height: 350px;
        background-image: url('../img/jumbotron.jpg');
    }
    button {
        background-color: $backgroundFooter;
        margin-bottom: 20px;
        color: white;
        border: none;
        padding: 8px 20px;
        font-weight: 600;
    }
</style>