<template>
  <v-app>
   <TopHeader/>

    <v-main>
 
   <MainBody/>
   <about/>
     <portfolio/>
     <project/>
     <gallery/>
     <contactUs/>
     <Vuefooter/>
    </v-main>
  </v-app>
</template>

<script>
import TopHeader from './components/header';
import about from './components/about';
import MainBody from './components/MainCom';
import portfolio from './components/portfolio';
import project from './components/project';
import gallery from './components/gallery';
import contactUs from './components/contactUs';
import Vuefooter from './components/footer';


export default {
  name: 'App',

  components: {
    MainBody,
    TopHeader,
    about,
    portfolio,
    project,
    gallery,
    contactUs,
    Vuefooter
    
  
  },

  data: () => ({
    //
  }),
};
</script>
