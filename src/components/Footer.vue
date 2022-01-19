<template>
    <footer class="jumbotron">
        <div class="container">
            <div class="content_wrapper">
                <div class="footer-contacts">
                    <Logo class="footer_logo" />
                    <p>A Functional HTML Template for Corporate & Business</p>
                    <div class="links">
                        <div class="single-link">
                            <span class="footer-icons">
                                <i class="fas fa-phone"></i>
                            </span>
                            <a href="#">+1 (305) 1234-5678</a>
                        </div>
                        <div class="single-link">
                            <span class="footer-icons">
                                <i class="fas fa-envelope"></i>
                            </span>
                                <a href="#">hello@example.com</a>
                        </div>
                        <div class="single-link">
                            <span class="footer-icons">
                                <i class="fas fa-map-marker-alt"></i>
                            </span>
                            <a href="#">Main Avenue,987</a>
                        </div>
                    </div>
                            <a class="empty_btn" href="#">get in touch</a>

                </div>
                <div class="info-row">
                    <!-- qui ci andranno le cards  -->
                    <div class="footer-card">
                        <div class="filter-wrapper">
                            <h3>ABOUT</h3>
                            <ul>
                                <li>
                                    <span class="card-icons"><i class="fas fa-chevron-right"></i></span>
                                    <a href="#">The company</a>
                                </li>
                            </ul>
                        </div>
                    </div>
                    <div class="footer-card">
                        <h3>TRANSPORT</h3>
                    </div>
                    <div class="footer-card">
                        <h3>SUPPORT</h3>
                    </div>
                </div>
            </div>
        </div>
        <!-- end container -->

    </footer>
</template>

<script>
import Logo from './Logo.vue';
export default {

    name:'Footer',

    components:{
        Logo,
    },
}

</script>

<style lang="scss" scoped>
@import '../style/variables.scss';
.jumbotron{
    width:100%;
    // test
    height: 720px;
    background-image: url('../assets/img/bg-10.jpg');
    background-position: center;
    background-size: cover;

    .content_wrapper{
        width: 100%;
        height: 100%;
        padding: 100px 0;
        color:$brand_secondary_text;
        display: flex;
        // test
        border: 1px solid white;
        .footer-contacts{
            width: 25%;
            height:100%;
            .footer_logo{
                font-size:23px;
                margin-bottom:30px;
            }
            .links{
                margin-top:30px;
                margin-bottom: 50px;
                .single-link{
                    margin-bottom: 20px;
                }
                .footer-icons{
                    margin-right:15px;
                    
                }
            }
        }
        .info-row{
            width: 75%;
            height: 100%;
            display: flex;
            justify-content: space-between;
            // COMPONENTE
            .footer-card{
                width:calc((100% / 3) - 18px);
                height: 100%;
                 background: rgba(80, 81, 86, 0.5);
                 border-radius:10px;
                 padding: 40px 20px;
                 h3{
                     color: white;
                     margin-bottom: 30px;
                 }
                // test
                border: 1px solid red;
                .filter-wrapper{
                    width:100%;
                    height: 100%;
                    backdrop-filter:opacity(0.6);
                }

                .card-icons{
                    margin-right: 15px;
                }
                
                
            }
        }
    }
}

</style>