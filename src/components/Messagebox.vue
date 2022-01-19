<template>
    <section class="message_section">
        <div class="container">
            <div class="content_wrapper">
                <div class="message_content">
                    <div class="message_content_info">
                            <h5>send a message</h5>
                             <div class="special_titles_variant">
                                Get in
                                <span class="special_text_variant">Touch</span>
                            </div>
                            <p class="paragraph">We will respond to you message as soon as possible.</p>
                    </div>
                    <div class="forms">
                        <form action="#">
                            <input class="form_style" type="text" placeholder="Name">
                            <input class="form_style" type="email" placeholder="email"><br>
                            <input class="form_style" type="text" placeholder="Phone">
                            <span class="special">
                                <input class="form_style" type="text" placeholder="More info">
                                <span class="icons chevron"><i class="fas fa-chevron-down"></i></span>
                            </span>
                            <div class="area_container">
                                <input class="message_area" type="text" placeholder="Message">
                            </div>
                        </form>
                        <a class="main_btn" href="#">send</a>
                    </div>
                    <!-- end forms -->
                </div>
                <div class="info_box">
                    <h3>Example inc.</h3>
                    <p class="paragraph">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                    <p class="paragraph">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                    <div class="contacts">
                        <div class="single_contact">
                            <span class="round_icons">
                               <i class="fas fa-phone"></i>
                            </span>
                            <a href="#">+1 (305) 1234-5678</a>
                        </div>
                         <div class="single_contact">
                            <span class="round_icons">
                               <i class="fas fa-envelope"></i>
                            </span>
                            <a href="#">hello@example.com</a>
                        </div>
                        <div class="single_contact">
                            <span class="round_icons">
                               <i class="fas fa-map-marker-alt"></i>
                            </span>
                            <a href="#">Main Avenue,987</a>
                        </div>
                        <div class="contact_btn">
                            <a class="empty_btn" href="#">wiew map</a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name:'Messagebox',
}
</script>

<style lang="scss" scoped>
@import '../style/variables.scss';
@import '../style/common.scss';

.message_section{
    width: 100%;
    background-color: $brand_background_color;
    padding: 100px 0;
    
    .content_wrapper{
        width: 100%;
        height: 100%;
        display: flex;
        .message_content{
            width: 70%;
            height: 100%;
            .message_content_info{
                width: 70%;
            }
            .forms{
                margin: 40px 0;
            }
        }
        .info_box{
            width:30%;
            height: 100%;
            h3{
                font-size: 23px;
            }
            p{
                margin:22px 0;
            };
            .contacts{
                padding: 5px 0;
               
                .single_contact{
                    font-size: 20px;
                    color:$brand_special_text;
                    margin: 25px 0;

                        .round_icons{
                    font-size: 20px;
                    color: $brand_primary_button;
                    background-color:#cce3de;
                    width:45px;
                    height: 45px;
                    border-radius: 50%;
                    display:inline-block;
                    text-align: center;
                    line-height: 45px;
                    margin-right: 20px;
                    }
                }
                .contact_btn{
                    margin-top: 50px;
                    a{
                        color:$brand_primary_button;
                    }
                }
                
            }
            
        }
    }

    .area_container{
        width: 100%;
        padding-right: 49px;
        margin-bottom: 35px;
        
    }

   
    .special{
        position: relative;
        display: inline;
    }
    .chevron{
        position: absolute;
        bottom: 0;
        right: 30px;
        color: $brand_secondary_text;
    }
    .message_area{
        width: 100%;
        padding:16px 170px 120px 16px;
        border-radius: 5px;
        margin: 10px 0;
        border:none;
        font-size: 18px;
        background-color: $brand_forms;
        color: $brand_secondary_text;

    }
}
// END MESSAGE BOX





</style>