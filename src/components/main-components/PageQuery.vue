<script>
import { store } from "../../store.js";
export default {
  name: "PageQuery",
  data() {
    return {
      store,
    };
  },
};
</script>

<template>
  <div class="query">
    <select
      name="category"
      id="category"
      v-model="store.categoryQuery"
      @change="$emit(`search`)"
    >
      <option disabled value="">Choose category</option>
      <option value="Breaking Bad">Breaking Bad</option>
      <option value="Better Call Saul">Better Call Saul</option>
      <option value="">Tutti</option>
    </select>
  </div>
</template>

<style lang="scss" scoped>
.query {
  font-size: 1.5rem;
  select {
    margin-left: 1rem;
    font-size: 1rem;
    padding: 0.5rem;
    border-radius: 6px;
  }
}
</style>
