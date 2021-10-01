<template>
  <div class="container-hero" :style="{'background-image': 'url(' + heroImg + ')'}"></div>
</template>

<script>
export default {
    name:'Hero',
    props: [
      'heroImg'
    ]
}
</script>

<style lang="scss" scope>
.container-hero{
    
    background-position: center top;
    background-size: cover;
    height: 25rem;
    width: 100%;
}

</style>