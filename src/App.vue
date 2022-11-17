<template>
  <div id="app">
    <div class="content">
      <MobileView v-if="!isDesktop" />
      <DesktopView v-else />
    </div>
    <FooterView />
  </div>
</template>

<script>
import './assets/styles/normalize.css';
import './assets/styles/fonts.css';
import './assets/styles/tablet.scss';
import MobileView from './components/MobileView.vue';
import FooterView from './components/FooterView.vue';
import DesktopView from './components/DesktopView.vue';
const throttle = require('lodash.throttle');


export default {
  name: 'App',
  components: {
    MobileView,
    FooterView,
    DesktopView
  },
  data() {
    return {
      isDesktop: false,
    }
  },
  methods: {
    calcIsDesktop() {
      this.isDesktop = window.innerWidth >= 1200;
    }
  },
  mounted() {
    window.addEventListener('resize', throttle(this.calcIsDesktop, 1000))
  },
  beforeDestroy() {
    window.removeEventListener('resize', this.calcIsDesktop);
  }
}
</script>

<style lang="scss">
html, body {
  height: 100%;
  background: #dd0d1d;
}
#app {
  height: 100%;
  margin: 0 auto;
}

.container {
  max-width: 375px;
  padding: 0 30px;
  margin: 0 auto;
}

@media screen and (min-width: 768px) {
  .container {
    max-width: 768px;
  }
}
@media screen and (min-width: 1200px) {
  .container {
    max-width: 1200px;
  }
}

</style>
