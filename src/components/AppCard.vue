<script>
export default {
  props: {
    thumb: String,
    series: String,
  },
};
</script>

<template>
  <div class="card">
    <img :src="thumb" alt="" />
    <h3>{{ series }}</h3>
  </div>
</template>

<style lang="scss" scoped>
.card {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  width: calc(100% / 6);
  margin-top: 30px;
  cursor: pointer;

  img {
    width: 80%;
  }
  h3 {
    color: rgb(189, 181, 181);
    font-size: 0.7rem;
    font-family: Arial, Helvetica, sans-serif;
  }
}
</style>
