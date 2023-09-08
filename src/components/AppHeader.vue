<script>
export default {
  data() {
    return {};
  },
};
</script>

<template>
  <header>
    <div><img src="../../public/img/dc-logo.png" /></div>
    <div>
      <ul>
        <li>CHARATERS</li>
        <li>COMICS</li>
        <li>MOVIES</li>
        <li>TV</li>
        <li>GAMES</li>
        <li>COLLECTIBLES</li>
        <li>VIDEOS</li>
        <li>FANS</li>
        <li>NEWS</li>
        <li>SHOP</li>
      </ul>
    </div>
  </header>
</template>
<style lang="scss" scoped>
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 100%;
  height: 80px;

  img {
    width: 75px;
  }

  ul {
    display: flex;
    gap: 1rem;

    li {
      list-style: none;
      font-weight: bolder;
      font-family: Arial, Helvetica, sans-serif;
      font-size: 0.8rem;
    }
  }
}
</style>
