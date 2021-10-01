<template>
    <div class="general-content-formatting">
        <button class="current-series">Current Series</button>
        <ul class="comics">

            <Card v-for="(comic,index) in myJson" :key="index" :card="comic" />


        </ul>
        <button>Load More</button>

    </div>
</template>

<script>
import Card from '../components/Card.vue'
import json from './dc-comics.json'
export default {
    name:'RecentSeries',
    components:{
        Card,
    },
    data(){
        return{
            myJson: json
        }
    },
    
}
</script>

<style lang="scss" scoped>

@import '../style/variables';

.general-content-formatting{
    text-align: center;
    margin: .9375rem auto;
    position: relative;

    button{
        
        color: white;
        font-weight: bold;
        font-size: .875rem;
        width: 12.5rem;
        height: 1.875rem;
        background-color: $site-features_primary_background_color;
        border: 0 ;
    }
    .current-series{
        position: absolute;
        top: -2.1875rem;
        left: 0;
        font-size: 1.25rem;
        
    }
    .comics{
        display: flex;
        flex-wrap: wrap;
        margin: 1.25rem 0;
        list-style: none;
        align-items: flex-start;
    }
}
</style>