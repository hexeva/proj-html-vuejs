<template>

<div class="nexgen">
     <div class="logo-wrapper">
        <div class="nex">nex</div>
        <div class="gen">gen</div>
    </div>
</div>
   
</template>

<script>
export default {
    name:'HeaderLogo',
}
</script>

<style lang="scss" scoped>
@import '../style/variables.scss';

.nexgen{
    width: 150px;
    height: 50px;
    text-transform: uppercase;
    font-size: 20px;
    font-weight: 700;
    letter-spacing: 5px;
    
    .logo-wrapper{
        width: 100%;
        height: 100%;
        display: flex;
        align-items: center;
        .nex{
            width:50%;
            height: 100%;
            display: flex;
            justify-content: flex-end;
            align-items: center;
            color: $brand_logo_text;
            background-color:$brand_logo_background;
            filter:opacity(0.7);
            border-top-left-radius:50%;
            border-bottom-left-radius:50%;
           
        }

        .gen{
            width: 50%;
            height: 100%;
            display: flex;
            align-items: center;
            color: $brand_logo_variant;
        }
    }
}



</style>