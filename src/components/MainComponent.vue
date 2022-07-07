<template>
  <section class="content">
    <JumbotronComponent />
    <CurrentSeriesComponent />
  </section>
</template>

<script>

import JumbotronComponent from './JumbotronComponent.vue'
import CurrentSeriesComponent from './CurrentSeriesComponent.vue'

export default {
    name: "MainComponent",
    components: { 
      JumbotronComponent,
      CurrentSeriesComponent 
    }
}
</script>

<style lang="scss" scoped>
    @import '../style/variables.scss';
    section{
        background-color: $secondary-color;
        color: white;
    }
</style>
