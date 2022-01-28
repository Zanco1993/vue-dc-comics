<template>
  <div id="app">
    <header-box :linkNav="prova"/>
    <jumbotron/>
    <card-box/>
    <footer-box/>
  </div>
</template>

<script>
import HeaderBox from './components/HeaderBox.vue'
import FooterBox from './components/FooterBox.vue'
import Jumbotron from './components/Jumbotron.vue'
import CardBox from './components/CardBox.vue'


export default {
  name: 'App',
  components: {
    HeaderBox,
    FooterBox,
    Jumbotron,
    CardBox
  },
  data() {
    return {
      prova: [
        'CHARACTERS',
        'COMICS',
        'MOVIES',
        'TV',
        'GAMES',
        'COLLECTIBLES',
        'VIDEOS',
        'FANS',
        'NEWS',
        'SHOP'
      ]
    }
  }
}
</script>

<style lang="scss">
@import './style/main.scss';
@import url('https://fonts.googleapis.com/css2?family=Roboto&display=swap');
</style>
