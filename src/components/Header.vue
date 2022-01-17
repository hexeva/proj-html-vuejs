<template>
    <header>
        <HeaderTop />
        <!-- jumbotron -->
        <section>
            <div class="jumbotron">
                <!-- Nav bar -->
                <div class="container">
                    <nav class="header_menu">
                        <div class="logo">
                            <!-- COMPONENTE LOGO -->
                            <HeaderLogo />
                        </div>
                        <div class="nav_menu">
                            <ul class="nav_links">
                                <li>
                                    <a href="#">HOME</a>
                                </li>
                                <li>
                                    <a href="#">SERVICES</a>
                                </li>
                                <li>
                                    <a href="#">SKILLS</a>
                                </li>
                                <li>
                                    <a href="#">PARTNERS</a>
                                </li>
                                <li>
                                    <a href="#">BLOG</a>
                                </li>
                                <li>
                                    <a href="#">GET IN TOUCH</a>
                                </li>
                            </ul>
                        </div>
                    </nav>
                    <!-- end header menu -->
                    <div class="logistic_wrapper">
                        <div class="logistic_title">
                                <h1><span>Logistics</span> that goes further.</h1>
                            <div class="logistic_description">
                                For 20 years working with the most innovative in the field of transport.
                            </div>
                            <div class="logistic_buttons">
                                <a class="main_btn" href="#">GET IN TOUCH</a>
                                <a class="empty_btn" href="#">READ MORE</a>
                            </div>
                        </div>
                        
                    </div>
                </div>
                <!-- end container -->
            </div>
            <!-- end jumbotron -->
        </section>
    </header>
</template>

<script>
import HeaderTop from "./HeaderTop.vue";
import HeaderLogo from "./HeaderLogo.vue";



export default {
    name:'Header',
    components:{
        HeaderTop,
        HeaderLogo,
    },
}
</script>

<style lang="scss" scoped>
@import '../style/variables.scss';
@import '../style/common.scss';

.jumbotron{
    width:100%;
    // test
    height: 750px;
    background-image:url('../assets/img/jumbo.jpg');
    background-repeat: no-repeat;
    background-position: center;
    filter: brightness(0.9);

        .header_menu{
            width:100%;
            // test
            height: 90px;
            display: flex;
            color: white;
            .logo{
                width:40%;
                height: inherit;
                display: flex;
                justify-content: center;
                align-items: center;
            }
            .nav_menu{
                width: 60%;
                height: inherit;
                .nav_links{
                    display: flex;
                    height: inherit;
                    align-items: center;
                    justify-content: space-evenly;
                }

            }
        }
        // HEADER BOTTOM
        .logistic_wrapper{
            width: 100%;
            height: 100%;
            position: relative;

                .logistic_title{
                    width: 35%;
                    position: absolute;
                    top: 90px;
                    right: 100px;

                    h1{
                        font-size: 70px;
                        color: white;
                        
                        span{

                            text-decoration:underline;
                            text-decoration-color: $brand_primary_button;
                            text-decoration-thickness: 10px;
                        }
                    }
                    .logistic_description{
                        font-size: 25px;
                        color: #b7b9c6;
                        margin:25px 0;
                    }

                    .logistic_buttons{
                        margin: 55px 0;
                        a{
                            margin-right:20px;
                        }
                    }
                }
        }
        // end wrapper
}


</style>