<template>
  <v-app>
      <Navbar />
      <transition name="slide" mode="out-in">
        <router-view></router-view>
      </transition>
  </v-app>
</template>

<script>
import Navbar from './components/Navbar.vue';

export default{
  components:{
    Navbar
  }
}

</script>

<style lang="scss">
  #routerlinks{
    display:inline-block;
    padding:20px;
    color:#ffffff;
    text-decoration: none;
  }
  .slide-enter-active,
  .slide-leave-active{
    transition: opacity .5s, transform .5s;
  }
  .slide-enter,
  .slide-leave-to{
    opacity:0;
  }

html {
  scroll-behavior: smooth;
}
</style>