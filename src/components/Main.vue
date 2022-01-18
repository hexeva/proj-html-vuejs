<template>
    <main>
        <!-- FIRST SECTION -->
        <section class="contents">
            <div class="container">
                <div class="services">
                    <div class="logistic cols">
                        <h5>OUR BUSINESS AREAS</h5>
                        <h2>Logistic Services</h2>
                        <p class="paragraph">We are leaders in providing logistic services with a set of cutting edge technologies and a team of experienced and renowned professionals</p>
                        <div class="qualities">
                            <!-- sono pulsanti? -->
                            <a class="section_btn" href="#">Tradition</a>
                            <a class="section_btn" href="#">Quality</a>
                            <a class="section_btn" href="#">Security</a>

                            <div class="info_service">
                                <a class="main_btn" href="#">READ MORE</a>
                            </div>

                        </div>
                    </div>
                    <div class="technology cols">
                        <div class="custom_card">
                            <div class="img_card">
                                <img src="../assets/img/gallery-3.jpg" alt="statistic app img">
                            </div>
                            <div class="card_content">
                                <h3>Technology</h3>
                                <p class="paragraph">Focused on developing technology solutions adapted to our clien's needs</p>
                            </div>
                        </div>
                    </div>
                    <div class="transport cols">
                        <div class="custom_card">
                            <div class="img_card">
                                <img src="../assets/img/gallery-5.jpg" alt="package img">
                            </div>
                            <div class="card_content">
                                <h3>Transport</h3>
                                <p class="paragraph">We develop operational strategies to improv logistical efficiency.</p>
                            </div>
                        </div>
                    </div>
                </div>
                
            </div>
        </section>
        <!-- END FIRST SECTION -->
        <!-- SECOND SECTION -->
        <section class="section_about">
            <!-- component -->
            <DotDecoration class="up" />
            <div class="company">
                <div class="company_info">
                    <h5>about the network</h5>
                    <div class="special_titles">
                        <span class="special_text">the</span>
                        Company
                    </div>
                    <p class="special_paragraph">With all of this expertise and capability comes an unrivalled commitment to customer service.</p>
                    <!-- SINGLE PERCENTAGE -->
                    <div class="company_percentages">
                        <div class="single_percentage">
                            <div class="percent">0<span>%</span></div>
                            <div class="percentage_info">
                                <h3>Leadership</h3>
                                <p class="special_paragraph">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                            </div>
                        </div>
                        <div class="single_percentage">
                            <div class="percent">0<span>%</span></div>
                            <div class="percentage_info">
                                <h3>Psycology</h3>
                                <p class="special_paragraph">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                            </div>
                        </div>
                        <div class="single_percentage">
                            <div class="percent one">1<span>%</span></div>
                            <div class="percentage_info">
                                <h3>Flexibility</h3>
                                <p class="special_paragraph">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <div class="company_img">
                <img src="../assets/img/about-5.jpg" alt="skygrape img">
            </div>
            <DotDecoration class="down" />
        </section>
        <!-- END SECOND SECTION -->
        <!-- SUPPORTED SECTION -->
         <div class="supported">
                <div class="container">
                    <div class="supported_wrapper">
                        <div class="supported_logo less">
                            <img src="../assets/img/logo-5.png" alt="less logo">
                        </div>
                        <div class="supported_logo">
                            <img src="../assets/img/logo-1.png" alt="woo commerce logo">
                        </div>
                        <div class="supported_logo">
                            <img src="../assets/img/logo-2.png" alt="worldpress logo">
                        </div>
                        <div class="supported_logo">
                            <img src="../assets/img/logo-3.png" alt="pingdom logo">
                        </div>
                        <div class="supported_logo">
                            <img src="../assets/img/logo-4.png" alt="jquery logo">
                        </div>
                        <div class="supported_logo less">
                            <img src="../assets/img/logo-5.png" alt="less logo">
                        </div>
                    </div>
                </div>
            </div>
            <!-- END SUPPORTED SECTION -->

            <!-- EDITORIAL SECTION -->
            <section class="editorials">
                <div class="container">
                    <div class="content_wrapper">
                        <div class="news">
                            <h5>our editorial content</h5>
                             <div class="special_titles_variant">
                                Latest
                                <span class="special_text_variant">News</span>
                            </div>
                            <p class="paragraph">Every week we publish content about what is best in the business world.</p>
                        </div>
                        <div class="news_btn">
                            <a class="main_btn" href="">see all</a>
                        </div>
                    </div>
                    <!-- EDITORIAL CARDS -->
                    <div class="card_wrapper">
                        <!-- single card -->
                        <div class="editorial_card left">
                            <div class="card_title">Increasing creativity is possible for everyone</div>
                        </div>
                        <div class="editorial_card center">
                            <div class="card_title">Increasing creativity is possible for everyone</div>
                        </div>
                        <div class="editorial_card right">
                            <div class="card_title">Increasing creativity is possible for everyone</div>
                        </div>
                    </div>
                </div>
                <!-- end container -->
            </section>
            <!-- END EDITORIAL SECTION -->
            <!-- NEWSLETTERS -->
            <Newsletters />
            <!-- END NEWSLETTERS -->
    </main>
    <!-- END MAIN -->
</template>

<script>
import DotDecoration from './DotDecoration.vue';
import Newsletters from './Newsletters.vue';

export default {
    name:'Main',
    components:{
        DotDecoration,
        Newsletters,
    },
}
</script>


<style lang="scss" scoped>
    @import '../style/variables.scss';
    @import '../style/common.scss';


    .contents{
        width:100%;
        background-color: $brand_background_color;
        padding-top:50px;
        padding-bottom: 100px;
        

        .services{
            display: flex;
            padding: 70px 0;
            justify-content: space-between;

            .logistic{
                padding-right:20px;
                
                h2{
                    margin: 30px 0;
                    font-size:45px;
                }

                .qualities{
                    margin-top:40px;
                    .info_service{
                        margin-top:40px;
                    }
                }
            }
            .technology{
                margin: 0 30px;
            }
             // CUSTOM CARDS
            .custom_card{
                    width:100%;
                    height: 100%;
                    background-color: white;
                    border-radius: 10px;
                    padding: 50px 15px;
                    .img_card{
                        width: 70%;
                        margin: auto;
                    }
                    .card_content{
                        width: 70%;
                        margin: auto;
                        h3{
                            font-size:25px;
                            margin:25px 0;
                        }
                    }
                }
         // end card
        }
    }
    // END FIRST SECTION

    // SECOND SECTION
    .section_about{
        width:100%;
        height: 950px;
        display:flex;
        position: relative;
        
        .company{
            width:45%;
            height: 100%;
            padding: 100px 0;
            background-color: $brand_background_second;
            color:$brand_primary_text;
            display: flex;
            justify-content: flex-end;
            .company_info{
                width: 60%;
                height: inherit;
               h5{
                   margin: 35px 0;
               }
               p{
                   margin: 35px 0;
               }
               .single_percentage{
                   display: flex;
                   height: 110px;
                   margin: 70px 0;
                   p{
                       margin: 0;
                   }
                   .percentage_info{
                       padding-top:7px;
                       h3{
                           font-size: 25px;
                           margin-bottom: 25px;
                       }
                   }

               }
            }  
        }
        // END COMPANY
        .company_img{
            width: 55%;
            height: 100%;
            overflow: hidden;
        }
    }
    // END SECOND SECTION

    // SUPPORT SECTION
    .supported{
        padding: 120px 0;
        background-color: $brand_background_color;
        .supported_wrapper{
            display: flex;
            justify-content: space-between;
            align-items: center;
            .supported_logo{
                width: 100px;
                img{
                    filter:invert(0.7);
                }
            }
            .less{
                    width: 60px;
                }
        }  
    }
    //END SUPPORT SECTION

    // EDITORIAL SECTION
    .editorials{
        background-color: white;
        width: 100%;
        padding: 120px 0;
        

        .content_wrapper{
            display: flex;
            margin-bottom: 30px;
            .news{
                width:80%;
                padding:30px 0;
            }
            .news_btn{
                width:20%;
                text-align: right;
                padding-top:177px;
            }
        }
        // editorial cards
        .card_wrapper{
            width: 100%;
            display: flex;
            justify-content: space-between;
            .editorial_card{
                width:calc((100% / 3) - 20px);
                // test
                height: 400px;
                background-position: center;
                background-size: cover;
                background-repeat: no-repeat;
                border-radius: 10px;
                overflow: hidden;
                
                .card_title{
                    color: white;
                    font-size: 24px;
                    text-align: center;
                    padding-top:302px;
                    height: 100%;
                    backdrop-filter:brightness(0.5);
                }
            }
            .left{
                background-image: url("../assets/img/news-1.jpg");

            }
            .center{
                background-image: url("../assets/img/news-2.jpg");

            }
            .right{
                background-image: url("../assets/img/news-3.jpg");

            }
        }
    }

    // END EDITORIAL SECTION



</style>