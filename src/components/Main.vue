<template>
    <main>
        <!-- FIRST SECTION -->
        <section class="contents">
            <div class="container">
                <div class="services">
                    <div class="logistic cols">
                        <h5>OUR BUSINESS AREAS</h5>
                        <h2>Logistic Services</h2>
                        <p>We are leaders in providing logistic services with a set of cutting edge technologies and a team of experienced and renowned professionals</p>
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
                                <p>Focused on developing technology solutions adapted to our clien's needs</p>
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
                                <p>We develop operational strategies to improv logistical efficiency.</p>
                            </div>
                        </div>
                    </div>
                </div>
                
            </div>
        </section>
        <!-- END FIRST SECTION -->
        <!-- SECOND SECTION -->
        <section class="section_about">
            <div class="company">
                <div class="company_info">
                    <h5>about the network</h5>
                    <div class="special_titles">
                        <span class="special_text">the</span>
                        Company
                    </div>
                    <p>With all of this expertise and capability comes an unrivalled commitment to customer service.</p>
                    <!-- SINGLE PERCENTAGE -->
                    <div class="company_percentages">
                        <div class="single_percentage">
                            <div class="percent">0<span>%</span></div>
                            <div class="percentage_info">
                                <h3>Leadership</h3>
                                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                            </div>
                        </div>
                        <div class="single_percentage">
                            <div class="percent">0<span>%</span></div>
                            <div class="percentage_info">
                                <h3>Psycology</h3>
                                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                            </div>
                        </div>
                        <div class="single_percentage">
                            <div class="percent one">1<span>%</span></div>
                            <div class="percentage_info">
                                <h3>Flexibility</h3>
                                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <div class="company_img">COMPANY img</div>

        </section>
        <!-- END SECOND SECTION -->
    </main>
    <!-- END MAIN -->
</template>

<script>
export default {
    name:'Main',
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
        
        p{
            color:$brand_secondary_text;
        }

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
        display:flex;
        
        .company{
            width:45%;
            height: 100%;
            padding: 120px 0;
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
                   color: $brand_secondary_text;
               }
               .single_percentage{
                   display: flex;
                   height: 110px;
                   margin: 70px 0;
                   p{
                       margin: 0;
                       color: $brand_secondary_text;
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
        .company_img{
            width: 50%;
            height: 100%;
        }
    }
    // END SECOND SECTION



</style>