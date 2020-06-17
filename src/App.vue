<template>
  <div>
    <compHeader/>
    <compFeatured/>
    <compMenu/>
    <compCallUs/>
    <compNewsletter/>
    <compFooter/>
  </div>
</template>

<script>
import compHeader from './components/Header-footer/Header.vue'
import compFooter from './components/Header-footer/Footer.vue'
import compFeatured from './components/Featured/index.vue'
import compMenu from './components/Menu/index.vue'
import compCallUs from './components/CallUs/index.vue'
import compNewsletter from './components/Newsletter/index.vue'

  export default {
    components:{
      compHeader,
      compFeatured,
      compMenu,
      compFooter,
      compCallUs,
      compNewsletter
    }
  }
</script>

<style>
  @import './assets/style.css';
</style>