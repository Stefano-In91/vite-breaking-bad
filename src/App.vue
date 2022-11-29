<script>
import PageTitle from "./components/PageTitle.vue";
import PageQuery from "./components/main-components/PageQuery.vue";
import PageMain from "./components/PageMain.vue";

export default {
  components: {
    PageTitle,
    PageQuery,
    PageMain,
  },
};
</script>

<template>
  <header>
    <PageTitle />
  </header>
  <main>
    <div class="container">
      <PageMain />
    </div>
  </main>
</template>

<style lang="scss">
@import "./style/global.scss";
</style>
