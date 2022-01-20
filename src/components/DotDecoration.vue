<template>
   <div class="dot_container">
        <div class="dot">
            <div class="single_dot"></div>
            <div class="single_dot"></div>
            <div class="single_dot"></div>
            <div class="single_dot"></div>
            <div class="single_dot"></div>
            <div class="single_dot"></div>
            <div class="single_dot"></div>
            <div class="single_dot"></div>
            <div class="single_dot"></div> 
        </div>
         <div class="dot">
            <div class="single_dot"></div>
            <div class="single_dot"></div>
            <div class="single_dot"></div>
            <div class="single_dot"></div>
            <div class="single_dot"></div>
            <div class="single_dot"></div>
            <div class="single_dot"></div>
            <div class="single_dot"></div>
            <div class="single_dot"></div> 
        </div>
         <div class="dot">
            <div class="single_dot"></div>
            <div class="single_dot"></div>
            <div class="single_dot"></div>
            <div class="single_dot"></div>
            <div class="single_dot"></div>
            <div class="single_dot"></div>
            <div class="single_dot"></div>
            <div class="single_dot"></div>
            <div class="single_dot"></div> 
        </div>
        <div class="dot">
            <div class="single_dot"></div>
            <div class="single_dot"></div>
            <div class="single_dot"></div>
            <div class="single_dot"></div>
            <div class="single_dot"></div>
            <div class="single_dot"></div>
            <div class="single_dot"></div>
            <div class="single_dot"></div>
            <div class="single_dot"></div> 
        </div>
   </div>
</template>

<script>
export default {
    name:'DotDecoration',
}
</script>

<style lang="scss" scoped>
@import '../style/variables.scss';


.dot_container{
    height: 70px;
    display: flex;
    flex-direction: column;
    justify-content: space-around;
   
            .dot{
            width:150px;
            background-color: trasparent;
            display: flex;
            flex-wrap: wrap;
            justify-content: space-around;

            .single_dot{
                width: 7px;
                height: 7px;
                background-color:$brand_decorations;
                border-radius: 50%;
                display: inline-block;
                filter: opacity(0.5);
            }
        }
}
.up{
    position: absolute;
    top: -33px;
    left: 41%;
}
.down{
    position: absolute;
    bottom: -33px;
    left: 41%;
}

</style>