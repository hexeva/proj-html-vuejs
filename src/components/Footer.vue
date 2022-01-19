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
                    <!-- first section -->
                    <div class="footer-card">
                        <div class="filter-wrapper">
                            <h3>{{this.sectionOne.title}}</h3>
                            <ul>
                                <li v-for="(link,index) in sectionOne.links" :key="index">
                                    <span class="card-icons"><i class="fas fa-chevron-right"></i></span>
                                    <a :href="link.href">{{link.name}}</a>
                                </li>
                            </ul>
                        </div>
                    </div>
                    <!-- second section -->
                     <div class="footer-card">
                        <div class="filter-wrapper">
                            <h3>{{this.sectionTwo.title}}</h3>
                            <ul>
                                <li v-for="(link,index) in sectionTwo.links" :key="index">
                                    <span class="card-icons"><i class="fas fa-chevron-right"></i></span>
                                    <a :href="link.href">{{link.name}}</a>
                                </li>
                            </ul>
                        </div>
                    </div>
                    <!-- third section -->
                    <div class="footer-card">
                        <div class="filter-wrapper">
                            <h3>{{this.sectionThree.title}}</h3>
                            <ul>
                                <li v-for="(link,index) in sectionThree.links" :key="index">
                                    <span class="card-icons"><i class="fas fa-chevron-right"></i></span>
                                    <a :href="link.href">{{link.name}}</a>
                                </li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
            <div class="end-credits">
                <div>Enjoy the low price.We are tracking any intention of piracy.</div>
                <div>
                    <i class="far fa-copyright"></i> 2020 NEXGEN is Proudly Powered by <span>Codings</span>
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
    props:{
        sectionOne:Object,
        sectionTwo:Object,
        sectionThree:Object,
    },
}

</script>

<style lang="scss" scoped>
@import '../style/variables.scss';
.jumbotron{
    width:100%;
    background-image: url('../assets/img/bg-10.jpg');
    background-position: center;
    background-size: cover;
    padding-top:50px;
       

    .content_wrapper{
        width: 100%;
        padding: 100px 0;
        color:$brand_primary_text;
        display: flex;
      
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
                 background: rgba(80, 81, 86, 0.2);
                 border-radius:10px;
                 padding: 45px 40px;
                 h3{
                     color: white;
                     margin-bottom: 30px;
                     font-size: 23px;
                 }
                 li{
                     margin-bottom: 18px;
                 }
             
                .filter-wrapper{
                    width:100%;
                    height: 100%;
                    
                }

                .card-icons{
                    margin-right: 15px;
                }
                
                
            }
        }
    }
    .end-credits{
        color:#c0c3d0;
        display: flex;
        justify-content: space-between;
        align-items: flex-end;
        margin-top:50px;
        padding-bottom: 10px;
        span{
            color: $brand_special_text;
        }
    }
}

</style>