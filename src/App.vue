<template>
  <div id="app">
    <Header :navMenu="navData" />
    <Main />
    <Footer :sectionOne="firstSection" :sectionTwo="secondSection" :sectionThree="thirdSection" />

  </div>
</template>

<script>

import Header from"./components/Header.vue";
import Main from"./components/Main.vue";
import Footer from"./components/Footer.vue";



export default {
  name: "App",
  components: {
    Header,
    Main,
    Footer,
  },
  data:function(){
    return{
      // HEADER'S DATA
      navData:[
        {
          name:'HOME',
          href:'/#',
        },
         {
          name:'SERVICES',
          href:'/#',
        },
         {
          name:'SKILLS',
          href:'/#',
        },
         {
          name:'BLOG',
          href:'/#',
        },
        
      ],
      // FOOTER'S DATA
      firstSection:{
        title:"About",
        links:[
          {
            name:'The Company',
            href:"/#"
          },
          {
            name:'Institutional',
            href:'/#',
          },
          {
            name:'Social & Events',
            href:'/#',
          },
          {
            name:'Innovation',
            href:'/#',
          },
          {
            name:'Envirovment',
            href:'/#',
          },
          {
            name:'Technology',
            href:'/#',
          },
        ],
      },
      // end first section
      secondSection:{
        title:"Transport",
        links:[
          {
            name:'Industrialized',
            href:"/#"
          },
          {
            name:'Chemicals',
            href:'/#',
          },
          {
            name:'Packaged Liquids',
            href:'/#',
          },
          {
            name:'Construction',
            href:'/#',
          },
          {
            name:'Laminated Wood',
            href:'/#',
          },
          {
            name:'And others',
            href:'/#',
          },
        ],
      },
      // END SECOND SECTION
      // THIRD SECTION
       thirdSection:{
        title:"Support",
        links:[
          {
            name:'Responsability',
            href:"/#"
          },
          {
            name:'Terms of Use',
            href:'/#',
          },
          {
            name:'About Cookies',
            href:'/#',
          },
          {
            name:'Privacy Policy',
            href:'/#',
          },
          {
            name:'Accessibility',
            href:'/#',
          },
          {
            name:'Information',
            href:'/#',
          },
        ],
      },
    }
    // end return
  },
};
</script>

<style lang="scss">
@import './style/variables.scss';
@import './style/general.scss';
@import './style/common.scss';

</style>
