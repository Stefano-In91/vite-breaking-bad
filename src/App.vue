<script>
import PageTitle from "./components/PageTitle.vue";
import PageQuery from "./components/PageQuery.vue";
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
  <PageTitle />
  <PageQuery />
  <PageMain />
</template>

<style lang="scss">
@import "./style/global.scss";
</style>
