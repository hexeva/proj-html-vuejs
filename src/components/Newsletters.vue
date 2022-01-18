<template>
    <section class="jumbo_newsletters">
        <div class="newsletter_container">
            <div class="newsletter_wrapper">
                <div class="newsletters_titles">
                    <h5>newsletter</h5>
                    <div class="special_titles">
                        <span class="special_text">Know</span>
                        First
                    </div>
                    <p class="special_paragraph">Follow closely and receive content about our company and the news of the current marker.</p>
                </div>
                <div class="newsletter_form">
                        <input type="text" id="Name" name="Name" placeholder="Name"><br>
                        <input type="email" id="email" name="email" placeholder="Email">
                        <a class="main_btn" href="#">Subscribe</a>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name:'Newsletters',
}
</script>

<style lang="scss" scoped>
@import '../style/variables.scss';
@import '../style/common.scss';

.jumbo_newsletters{
    width: 100%;
    background-image: url('../assets/img/bg-1.jpg');
    background-position: center;
    padding: 140px 0;
    .newsletter_container{
        width: 50%;
        margin: auto;
        height: 100%;
        .newsletter_wrapper{
            width: 100%;
            height: 100%;
            display: flex;
            align-items: center;
            .newsletters_titles{
                width: 50%;
                margin-right: 20px;
                h5{
                    margin: 35px 0;
                }
                
            }
            .newsletter_form{
                width: 50%;
                
                input{
                    padding:13px 250px 13px 13px;
                    margin-bottom: 34px;
                    border-radius:5px;
                    box-shadow: none;
                    background-color:$brand_forms;
                    color: #787591;
                    font-size: 18px;
                    filter:opacity(0.8);
                    border: none;
                }
                
            }
        }
    }
}


</style>