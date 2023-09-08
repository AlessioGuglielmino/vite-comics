<script>
// IMPORTO I COMPONENTS DENTRO L'APP.VUE

import AppFooter from "./components/AppFooter.vue";
import AppHeader from "./components/AppHeader.vue";
import AppMain from "./components/AppMain.vue";

// ESPORTO  I COMPONENTS DENTRO L'APP.VUE

export default {
  components: { AppFooter, AppHeader, AppMain },
};
</script>

<template>
  <div class="wrapper">
    <AppHeader />
  </div>
  <AppMain />
  <AppFooter />
</template>

<style>
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

.wrapper {
  margin: 0 20%;
}
</style>
