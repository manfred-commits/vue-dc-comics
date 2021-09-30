<template>
    <div class="card-container">
        <img :src="card.thumb" :alt="card.type">
        
        <div class="series">
            <h5>{{card.series}}</h5>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Card',

    props: ['card']
}
</script>

<style lang="scss" scope>
.card-container{
    text-align: center;
    width: calc(100% / 6);
    padding: .625rem;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;

    img{
        object-fit: cover;
        object-position: center;
        width: 100%;
        height: 9.375rem;
    }
    h5{
        color: lightgrey;
        margin: .625rem;
    }
}
</style>