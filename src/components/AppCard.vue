<script>
export default {
  props: { card: Object },
};
</script>

<template>
  <div class="card">
    <img :src="card.thumb" alt="" />
    <h3>{{ card.series }}</h3>
  </div>
</template>

<style lang="scss" scoped>
.card {
  img {
    width: 100px;
  }
  h3 {
    color: whitesmoke;
  }
}
</style>
