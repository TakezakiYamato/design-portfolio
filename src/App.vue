<template>
  <v-app>
    <Header/>
    <Top/>
    <Skill/>
    <About/>
    <Footer/>
  </v-app>
</template>

<script>
import Header from './components/Header';
import Top from './components/Top';
import Skill from './components/Skill';
import About from './components/About';
import Footer from './components/Footer';

export default {
  name: 'App',
  components: {
    Header,
    Top,
    Skill,
    About,
    Footer
  },

  data: () => ({
    //
  }),
};
</script>
