<template>
    <div class="card-container">
        <img :src="card.thumb" :alt="card.type">
        <h5>{{card.series}}</h5>
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
    width: 100% /6;

    img{
        object-fit: cover;
        object-position: center;
        width: 100%;
    }
}
</style>