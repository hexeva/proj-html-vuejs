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
    </main>
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
                
                h5{
                    text-transform: uppercase;
                    color:$brand_special_text;
                }
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


</style>