<template>
  <div id="app">
    <HeaderContent />
  </div>
</template>

<script>
import HeaderContent from './components/HeaderContent.vue'

export default {
  name: 'App',
  components: {
    HeaderContent
  }
}
</script>

<style lang="scss">
@import './style/commons.scss'
</style>
