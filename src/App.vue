<template>
  <div id="app">
    <navbar></navbar>
    <hero></hero>
    <players></players>
    <features></features>
    <icons></icons>
    <footers></footers>
  </div>
</template>

<script>
import Navbar from '@/components/Navbar.vue'
import Hero from '@/components/Hero.vue'
import Players from '@/components/Players.vue'
import Features from '@/components/Features.vue'
import Icons from '@/components/Icons.vue'
import Footers from '@/components/Footer.vue'

export default {
  name: 'App',
  components: {
    Navbar,
    Hero,
    Players,
    Features,
    Icons,
    Footers
  }
}
</script>

<style lang="scss">
// darker blue: #1E2029
// dark blue: #393E5E
// yellow: #F8D643
// red: #ED5C5E
// white: #FFFFFF

@font-face {
  font-family: "FashionFetish";
  src: url("./assets/fonts/Fashion Fetish Regular.ttf");
}
#app {
  background-color: #1E2029;
  height: 100vh;
  font-family: '', sans-serif;
  color: #FFFFFF;
}

</style>
