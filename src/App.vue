<template>
  <div id="app">
    <header-box/>
    <jumbotron/>
    <footer-box/>
  </div>
</template>

<script>
import HeaderBox from './components/HeaderBox.vue'
import FooterBox from './components/FooterBox.vue'
import Jumbotron from './components/Jumbotron.vue'


export default {
  name: 'App',
  components: {
    HeaderBox,
    FooterBox,
    Jumbotron
    
  }
}
</script>

<style lang="scss">
@import './style/main.scss';
@import url('https://fonts.googleapis.com/css2?family=Roboto&display=swap');
</style>
