<template>
  <div id="app">
    <BaseHeader/>
    <BaseMain/>
    <BaseFooter/>
  </div>
</template>

<script>
import BaseFooter from './components/Footer/BaseFooter.vue'
import BaseHeader from './components/Header/BaseHeader.vue'
import BaseMain from './components/Main/BaseMain.vue'


export default {
  name: 'App',
  components: {
    BaseHeader,
    BaseMain,
    BaseFooter
    
  }
}
</script>

<style lang="scss">
@import './assets/style/global.scss';
</style>
