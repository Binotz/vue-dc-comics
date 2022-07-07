<template>
  <div id="app">
    <HeaderContent />
    <main>
      <MainComponent />
      <CTAComponent />
    </main>
    <footer>
      <FooterTopComponent />
      <FooterBottomComponent />
    </footer>
  </div>
</template>

<script>
import HeaderContent from './components/HeaderContent.vue'
import MainComponent from './components/MainComponent.vue'
import CTAComponent from './components/CTAComponent.vue'
import FooterTopComponent from './components/FooterTopComponent.vue'
import FooterBottomComponent from './components/FooterBottomComponent.vue'


export default {
  name: 'App',
  components: {
    HeaderContent,
    MainComponent,
    CTAComponent,
    FooterTopComponent,
    FooterBottomComponent
  }
}
</script>

<style lang="scss">
@import './style/commons.scss';
</style>
