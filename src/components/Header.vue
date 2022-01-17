<template>
    <header>
        <HeaderTop />
        <!-- jumbotron -->
        <section>
            <div class="jumbotron">
                <!-- Nav bar -->
                <div class="container">
                    <nav class="menu">
                        <div class="logo">NEXGEN</div>
                        <div class="nav_menu">
                            <ul>
                                <li>
                                    <a href="#">HOME</a>
                                </li>
                                <li>
                                    <a href="#">SERVICES</a>
                                </li>
                                <li>
                                    <a href="#">SKILLS</a>
                                </li>
                                <li>
                                    <a href="#">PARTNERS</a>
                                </li>
                                <li>
                                    <a href="#">BLOG</a>
                                </li>
                                <li>
                                    <a href="#">GET IN TOUCH</a>
                                </li>
                            </ul>
                        </div>
                    </nav>
                </div>
            </div>
        </section>
    </header>
</template>

<script>
import HeaderTop from "./HeaderTop.vue";


export default {
    name:'Header',
    components:{
        HeaderTop,
    },
}
</script>

<style lang="scss" scoped>
@import '../style/variables.scss';
@import '../style/common.scss';

.jumbotron{
    width:100%;
    // test
    height: 590px;
    background-image:url('../assets/img/jumbo.jpg');
    background-repeat: no-repeat;
    background-position: center;
    filter: brightness(0.5);

        .menu{
            width:100%;
            // test
            height: 100px;
            background-color: khaki;
            display: flex;
            .logo{
                width:40%;
            }
            .nav_menu{
                width: 60%;
                height: inherit;
                ul{
                    display: flex;
                    height: inherit;
                    align-items: center;
                    justify-content: space-between;
                }

            }
        }
}


</style>