<template>
  <div class="single-card-layout">
    <div class="single-card-content">
        <img :src="data.thumb">
        <span>{{ data.series.toUpperCase() }}</span>
    </div>
  </div>
</template>

<script>
export default {
    name: "SingleCardComponent",
    props:{
        data: Object
    }
}
</script>

<style lang="scss" scoped>
    .single-card-layout{
        margin: 0 15px;
        margin-bottom: 3rem;
        width: calc( (100% / 6) - 30px);
        
        img{
            width: 100%;
            margin-top: -80px;
            margin-bottom: 1rem;
            display: block;
            object-position: 0px 80px;
        }

        span{
            font-size: .9rem;
        }
    }
</style>
