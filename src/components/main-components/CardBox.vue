<script>
import { store } from "../../store.js";
import SingleCard from "./SingleCard.vue";

export default {
  name: "CardBox",
  components: {
    SingleCard,
  },
  data() {
    return {
      store,
    };
  },
};
</script>

<template>
  <div class="card-box">
    <SingleCard v-for="character in store.characters" :info="character" />
  </div>
</template>

<style lang="scss" scoped>
.card-box {
  margin-top: 1rem;
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
}
</style>
