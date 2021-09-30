<template>
    <footer>
        <div class="general-content-formatting top">

            <section class="footer-top">
                <div class="footer-top-menus">
                <div class="first-menu">
                    <div class="menu-top-block">
                    <h4>DC COMICS</h4>
                    <ul>
                        <li>
                            <a href="#">
                                Characters
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                Comics
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                Movies
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                TV
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                Games
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                Videos
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                News
                            </a>
                        </li>
                    </ul>
                    </div>

                    <div class="menu-bottom-block">
                    <h4>SHOP</h4>
                    <ul>
                        <li>
                            <a href="#">
                                Shop DC
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                Shop DC Collectibles
                            </a>
                        </li>
                    </ul>

                    </div>
                </div>
                
                <div class="menu">
                    <h4>DC</h4>
                    <ul>
                        <li>
                            <a href="#">
                                Terms Of Use
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                Privacy policy (New)
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                Ad Choices
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                Advertising
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                Jobs
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                Subscriptions
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                Talent Workshops
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                CPSC Certificates
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                Ratings
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                Shop Help
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                Contact Us
                            </a>
                        </li>
                    </ul>
                </div>
                <div class="menu">
                    <h4>SITES</h4>
                    <ul>
                        <li>
                            <a href="#">
                                DC
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                MAD Magazine
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                DC Kids
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                DC Universe
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                DC Power Visa
                            </a>
                        </li>
                    </ul>
                </div>
                </div>
                
            </section>
        </div>
        <div class="bottom">
            <section class="general-content-formatting footer-bottom">
                <div class="left-clm">
                    <button>SIGN-UP NOW!</button>
                </div>
                <div class="right-clm">
                    <h4>
                        <a href="#">
                            FOLLOW US
                        </a>
                    </h4>
                    <div class="footer-logo-socials">
                        <a href="#">
                            <img src="img/footer-facebook.png" alt="facebook link">
                        </a>
                    </div>
                    <div class="footer-logo-socials">
                        <a href="#">
                            <img src="img/footer-twitter.png" alt="twitter link">
                        </a>
                    </div>
                    <div class="footer-logo-socials">
                        <a href="#">
                            <img src="img/footer-youtube.png" alt="youtube link">
                        </a>
                    </div>
                    <div class="footer-logo-socials">
                        <a href="#">
                            <img src="img/footer-pinterest.png" alt="pinterest link">
                        </a>
                    </div>
                    <div class="footer-logo-socials">
                        <a href="#">
                            <img src="img/footer-periscope.png" alt="periscope link">
                        </a>
                    </div>
                </div>
            </section>
        </div>
    </footer>
</template>

<script>
export default {
    name:'Footer'
}
</script>

<style lang="scss" scoped>

@import '../style/variables.scss';


footer{
    background-image: url('../assets/footer-bg.jpg');
    background-position: center top;

    .top{
        flex-grow: 1;
        height: 100%;
        background-image: url('../assets/dc-logo-bg.png');
        background-repeat: no-repeat;
        background-position: center right;

        .footer-top{
            display: flex;
            align-items: flex-start;
            justify-content: space-between;


            .footer-top-menus{
                display: flex;
                flex-wrap: wrap;
                align-items: flex-start;
                width: 100%;
                padding: 0 0 2.8125rem;
                padding-left: 0rem;



                .first-menu{
                    padding: .625rem 0;
                    padding-right: .9375rem;
                }
                .menu{
                    padding: .625rem 1.25rem;
                }
                h4{
                    font-size: 1.25rem;
                    padding: .8125rem;
                    padding-left: 0rem;

                    color:white;
                }
                ul{
                    list-style: none;

                    li{
                        

                        a{
                            text-decoration: none;
                            color: grey;
                        }
                    }
                }
            }


        }

        
    }
    .bottom{
        flex-grow: 1;
        height: 100%;
        background-color: #303030;

        .footer-bottom{
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1.875rem 0;
            .left-clm{

                button{
                    padding: .625rem;
                    background-color: #303030;
                    border-color: $site-features_primary_background_color;
                    color: white;
                    font-weight: bold;
                    border-style: solid;
                }


            }
            .right-clm{
                display: flex;
                align-items: center;

                h4{

                    padding-right: 1.225rem;

                    a{
                        text-decoration: none;
                        color: $site-features_primary_background_color;
                    }
                }

                .footer-logo-socials{
                    padding: 0 .625rem 0;

                    &:last-child{
                        padding-right: 0;
                    }
                }
                
            }


        }
    }

}
</style>