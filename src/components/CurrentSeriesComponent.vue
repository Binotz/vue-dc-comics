<template>
  <section class="current-series">
    <div class="container">
        <div class="current-series-text">
            <span>CURRENT SERIES</span>
        </div>
        <div class="cards-container">
            <SingleCardComponent v-for="card,index in JsonData" :key="index" :data="card"/>
        </div>
        <div class="load-more-text">
            <a href="#">LOAD MORE</a>
        </div>
  </div>
  </section>
</template>

<script>
import SingleCardComponent from './SingleCardComponent.vue'
import JSONDataFromFile from './data/dc-comics.json'

export default {
    name: "CurrentSeriesComponent",
    components:{
        SingleCardComponent
    },
    data(){
        return{
            JsonData: JSONDataFromFile
        };
    }
}
</script>

<style lang="scss" scoped>
    @import '../style/variables.scss';

    .current-series{
        background-color: $secondary-color;
        padding: 5rem;
    }
    .container{
        position: relative;
    }
    .cards-container{
        display: flex;
        flex-wrap: wrap;
        margin-bottom: 2rem;
    }
    .current-series-text{
        padding: 1rem 2rem;
        background-color: $primary-color;
        position: absolute;
        top: -20%;
        left: 0;
        
        span{
            font-size: 2rem;
            font-weight: bold;
        }

    }
    .load-more-text{
        margin: 0 auto;
        text-align: center;
        a{
            padding: 1rem 2rem;
            background-color: $primary-color;
            color: white;
        }
    }
    
</style>
