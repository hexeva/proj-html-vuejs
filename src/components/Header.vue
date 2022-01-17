<template>
    <header>
        <HeaderTop />
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


</style>