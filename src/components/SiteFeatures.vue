<template>
  
<div class="features-line">
    <section class="general-content-formatting site-features">

        <ul>
            <li v-for="(feature,index) in features" :key="index">
                <a :href="feature.url">
                    <div class="container-img">
                        
                        <img :src="require('../assets/img/'+ feature.img)" :alt="feature.link.toUpperCase()">
                        
                    </div>
                    <h4>{{feature.link.toUpperCase()}}</h4>
                </a>
            </li>
        </ul>

    </section>
</div>

</template>

<script>
export default {
    name:'SiteFeatures',
    data() {
        return {
            features:    [
                {
                    img:'buy-comics-digital-comics.png',
                    url:'#',
                    link:'digital comics'
                },
                {
                    img:'buy-comics-merchandise.png',
                    url:'#',
                    link:'Dc merchandise'
                },
                {
                    img:'buy-comics-subscriptions.png',
                    url:'#',
                    link:'subscription'

                },
                {
                    img:'buy-comics-shop-locator.png',
                    url:'#',
                    link:'Comic shop locator'
                },
                {
                    img:'buy-dc-power-visa.svg',
                    url:'#',
                    link:'Dc power visa'

                }
                
            ]
            
        }
    }

}
</script>

<style lang="scss" scoped>
@import '../style/variables.scss';

.features-line{
    
    background-color: $site-features_primary_background_color;
    display: flex;
    align-items: center;

    .site-features{
        ul{
            list-style: none;
            display: flex;
            justify-content: space-around;
            align-items: center;
            li{
                padding: 1.875rem 0;

                a{
                    display: flex;
                    align-items: center;
                    color: white;
                    text-decoration: none;
                    font-weight: 400;


                    .container-img{
                        height: 60px;
                        img{
                            object-fit: cover;
                            width: 100%;
                            height: 100%;
                        }
                    }
                    h4{
                        padding: .3125rem;
                    }
                }
            }
        }

    }
    
}

</style>