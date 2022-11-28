<script>
import CardBox from "./main-components/CardBox.vue";
export default {
  name: "PageMain",
  components: {
    CardBox,
  },
};
</script>

<template>
  <div class="card-container">
    <div class="found">
      <h3>trovati sbabbari</h3>
    </div>
    <CardBox />
  </div>
</template>

<style lang="scss" scoped>
.card-container {
  background-color: white;
  margin-top: 1rem;
  padding: 2rem;
  .found {
    width: 100%;
    background-color: var(--secondary-color);
    padding: 1rem;
  }
}
</style>
