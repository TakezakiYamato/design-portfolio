<template>
  <v-app id=app>
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
<style>
/* Google fontの導入 */
@import url('https://fonts.googleapis.com/css2?family=Lato:wght@400;700&family=Montserrat:wght@500;600&family=Noto+Sans+JP&display=swap');
#app {
  font-family: 'Montserrat', sans-serif;
  color: #1D2B95;
}
</style>
