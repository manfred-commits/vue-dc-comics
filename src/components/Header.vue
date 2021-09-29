<template>
    <header>
        <div class="general-content-formatting">
            <nav>
                <div class="container-img">
                    <img src="@/assets/img/dc-logo.png" alt=" Detective Comics small logo">
                </div>
                
                <ul>
                    <li v-for="(component,index) in nav" :key="index" :class="{active : component.current==true}">
                        <a :href="component.url">{{component.name.toUpperCase()}}</a>
                    </li>
                </ul>            
            </nav>
        </div>
    </header>
</template>

<script>
export default {
    name:'Header',
    data() {
        return {
            nav:    [
                {
                    name:"characters",
                    url:"#",
                    current:false
                },
                {
                    name:"comics",
                    url:"#",
                    current:true
                },
                {
                    name:"movies",
                    url:"#",
                    current:false
                },
                {
                    name:"Tv",
                    url:"#",
                    current:false
                },
                {
                    name:"Games",
                    url:"#",
                    current:false
                },
                {
                    name:"Collectibles",
                    url:"#",
                    current:false
                },
                {
                    name:"Videos",
                    url:"#",
                    current:false
                },
                {
                    name:"Fans",
                    url:"#",
                    current:false
                },
                {
                    name:"News",
                    url:"#",
                    current:false
                },
                {
                    name:"Shop",
                    url:"#",
                    current:false
                },
            ]
            
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../style/variables.scss';
header{
    
    background-color: $nav_primary_background_color;
    
    nav{
        display: flex;
        align-items: center;
        width: 100%;
        justify-content: space-between;
        font-weight: bold;
        
        .container-img{
            
            height: 5rem;
            

            img{
                object-fit: cover;
                height: 100%;
                width: 100%;

            }

            
        }
        ul{
            display: flex;
            list-style: none;

            li:last-child{
               padding-right: 0rem; 
               margin-right: 0rem; 
            }

            li{
                padding: 2.5rem 0;
                margin: 0rem 1rem;
            
                &.active{
                    color: $active_color;
                    border-bottom: .1875rem solid $active_color;

                    a{
                    color: $active_color;

                    }
                }

                a{
                    color: $nav_primary_text_color;
                    text-decoration: none;
                }
            }
        }
    }
}
</style>