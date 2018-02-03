<template>
  <div class="hello">
    <main-header></main-header>
    <div class="content">
      <drawer class="col"></drawer>
      <v-card-title raised class="col content-main">
        <carousel :items="carouselItems"></carousel>
      </v-card-title>
    </div>
    <main-footer></main-footer>
  </div>
</template>

<script>
import MainHeader from '@/components/Header'
import Drawer from '@/components/Drawer'
import MainFooter from '@/components/Footer'
import Carousel from '@/components/Carousel'

export default {
  components: {
    MainHeader,
    Drawer,
    MainFooter,
    Carousel
  },
  name: 'HomePage',
  data () {
    return {
      msg: 'Welcome to Theo Class',
      carouselItems: [
        {
          src: '/static/1.jpg'
        },
        {
          src: '/static/2.jpg'
        },
        {
          src: '/static/3.jpg'
        },
        {
          src: '/static/5.jpg'
        }
      ]
    }
  }
}
</script>
<style>
  .content {
    margin-top: 64px !important;
    display: flex;
  }
  .content-main {
    width: 100%;
  }
</style>
