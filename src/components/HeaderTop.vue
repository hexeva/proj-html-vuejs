<template>
    <section class="top_page">
        <div class="container">
            <div class="top_info">
                <!-- left col -->
                <div class="left_col">
                    <div class="hours_info"> 
                        <span class="icons"><i class="fas fa-clock"></i></span>
                        Open Hours: Mon - Sat - 9:00 - 18:00</div>
                    </div>
                <!-- right col -->
                <div class="right_col">
                    <div class="tel_info">
                        <span class="icons"><i class="fas fa-phone"></i></span>
                        +1 (305) 1234-5678
                    </div>
                    <div class="mail">
                        <span class="icons"><i class="fas fa-envelope"></i></span>
                        hello@example.com
                    </div>
                    <div class="links">
                        <a href="#">
                            <span class="icons"><i class="fab fa-facebook-f"></i></span>
                        </a>
                        <a href="#">
                            <span class="icons"><i class="fab fa-twitter"></i></span>
                        </a>
                        <a href="#">
                            <span class="icons"><i class="fab fa-linkedin-in"></i></span>
                        </a>
                    </div>
                </div>
            </div>
            
        </div>
        
    </section>
</template>

<script>
export default {
    name:'HeaderTop',
}
</script>

<style lang="scss" scoped>
@import '../style/variables.scss';




.top_page{
    background-color:#293c4c;
    width: 100%;
    height: 40px;
    color: white;
    font-size: 13px;

        .top_info{
            display: flex;
            align-items: center;
            height: inherit;

            .left_col{
                width: 55%;
                display: flex;
                justify-content: flex-start;
            }
            .right_col{
                width: 45%;
                display: flex;
                justify-content: space-evenly;

                .links > a{
                    margin: 0 13px;
                }
            }
        }
        // end top_info
   
}


</style>