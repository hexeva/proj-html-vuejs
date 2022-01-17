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
                    <div class="technology cols">TECNOLOGY</div>
                    <div class="transport cols">TRANSPORT</div>
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
        padding: 50px 0;
        // test
        height: 800px;
        p{
            color:$brand_secondary_text;
        }

        .services{
            display: flex;
            padding: 10px 0;

            .logistic{
                padding-right:95px;
                
                h5{
                    text-transform: uppercase;
                    color:$brand_special_text;
                }
                h2{
                    margin: 30px 0;
                    font-size:40px;
                }

                .qualities{
                    margin: 30px 0;
                    .info_service{
                        margin: 40px 0;
                    }
                }

                
            }
        }

       
    }


</style>