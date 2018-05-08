<template>
  <div id="app">
    <div id="nav">
        <md-card>
          <md-card-actions>
            <div class="md-subhead">
              <span>Default Setup</span>
              <span>（</span>
              <span>默认设置</span>
              <span>）</span>
            </div>
            <md-button class="md-icon-button"
                      target="_blank"
                      href="https://github.com/surmon-china/vue-awesome-swiper/blob/master/examples/01-default.vue">
              <md-icon>code</md-icon>
            </md-button>
          </md-card-actions>
          <md-card-media>
            <!-- swiper -->
            <swiper>
              <swiper-slide class="bg-info">Slide 1</swiper-slide>
              <swiper-slide>Slide 2</swiper-slide>
              <swiper-slide>Slide 3</swiper-slide>
              <swiper-slide>Slide 4</swiper-slide>
              <swiper-slide>Slide 5</swiper-slide>
              <swiper-slide>Slide 6</swiper-slide>
              <swiper-slide>Slide 7</swiper-slide>
              <swiper-slide>Slide 8</swiper-slide>
              <swiper-slide>Slide 9</swiper-slide>
              <swiper-slide>Slide 10</swiper-slide>
            </swiper>
          </md-card-media>
        </md-card>

      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div>
    <router-view/>
  </div>
</template>

<script>
import { swiper, swiperSlide } from 'vue-awesome-swiper'

export default {
  components: {
    swiper,
    swiperSlide
  }
}
</script>

<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
#nav {
  padding: 30px;
  a {
    font-weight: bold;
    color: #2c3e50;
    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
