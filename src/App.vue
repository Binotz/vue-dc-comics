<template>
  <div id="app">
    <HeaderContent />
    <MainComponent />
    <CTAComponent />
  </div>
</template>

<script>
import HeaderContent from './components/HeaderContent.vue'
import MainComponent from './components/MainComponent.vue'
import CTAComponent from './components/CTAComponent.vue'

export default {
  name: 'App',
  components: {
    HeaderContent,
    MainComponent,
    CTAComponent
  }
}
</script>

<style lang="scss">
@import './style/commons.scss';
</style>
