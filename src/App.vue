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
  <h1>
    <AppHeader />
  </h1>
</template>
<style></style>
