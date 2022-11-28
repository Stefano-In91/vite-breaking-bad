<script>
import SingleCard from "./SingleCard.vue";
export default {
  name: "CardBox",
  components: {
    SingleCard,
  },
};
</script>

<template>
  <div class="card-box">
    <SingleCard />
    <SingleCard />
    <SingleCard />
    <SingleCard />
    <SingleCard />
    <SingleCard />
    <SingleCard />
    <SingleCard />
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
