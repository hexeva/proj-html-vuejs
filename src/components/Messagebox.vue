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

                            
                            <textarea class="textarea" name="Message" id="" cols="30" rows="10">Message</textarea>
                        </form>
                    </div>
                </div>
                <div class="info_box">
                    info box
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
    // test
    height: 500px;
    .content_wrapper{
        width: 100%;
        height: 100%;
        display: flex;
        .message_content{
            width: 70%;
            height: 100%;
            // test
            border-right: 1px solid black;
            .message_content_info{
                width: 70%;
            }
        }
        .info_box{
            width:30%;
            height: 100%;
        }
    }
    .special{
        position: relative;
    }
    .chevron{
        position: absolute;
        bottom: 0;
        right: 30px;
        color: $brand_secondary_text;
    }
}


</style>