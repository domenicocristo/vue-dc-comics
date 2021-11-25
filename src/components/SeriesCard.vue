<template>
    <div class="serie">
        <img :src="details.thumb" alt="serie">
        <h4>{{details.series}}</h4>
    </div>
</template>

<script>
export default {
  name: 'SeriesCard',
  props: {
      details: Object
  }
}
</script>

<style scoped lang="scss">
    .serie {
        width: calc(100% / 7);
        display: inline-block;
        margin: 10px;
        cursor: pointer;
        img {
            height: 170px;
            width: 170px;
        }
        img:hover {
           border: 5px solid #0182f9;
        }
    }
</style>