<script>
export default {
  name: "SingleCard",
  props: {
    info: Object,
  },
};
</script>

<template>
  <div class="card">
    <img :src="info.img" :alt="info.name" />
    <h2>{{ info.nickname }}</h2>
    <h3>{{ info.name }}</h3>
    <p>{{ info.status }}</p>
  </div>
</template>

<style lang="scss" scoped>
.card {
  display: flex;
  flex-wrap: wrap;
  text-align: center;
  width: calc(100% / 5);
  padding: 1rem;
  background-color: var(--primary-color);
  & * {
    width: 100%;
    margin-bottom: 0.5rem;
  }
  img {
    height: 300px;
    object-fit: cover;
  }
  p {
    color: darkgray;
  }
}
</style>
