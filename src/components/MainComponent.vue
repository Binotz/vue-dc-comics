<template>
  <section class="content">
    <div class="container">
    <span> Content Goes Here </span>
  </div>
  </section>
</template>

<script>
export default {
    name:"MainComponent"
}
</script>

<style lang="scss" scoped>
    @import '../style/variables.scss';
    section{
        background-color: $secondary-color;
        color: white;
        padding: 3rem;
    }
</style>
