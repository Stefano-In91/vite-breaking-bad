<script>
export default {
  name: "PageTitle",
  data() {
    return {
      logo: "src/assets/logo.png",
      title: "Breaking Api Bad",
    };
  },
};
</script>

<template>
  <div>
    <img :src="logo" :alt="title" />
    <h1>{{ title }}</h1>
  </div>
</template>

<style lang="scss" scoped>
div {
  display: flex;
  align-items: center;
  height: 8vh;
  padding: 1rem;
  img {
    height: 50px;
    margin-right: 2rem;
  }
  h1 {
    font-size: 3rem;
  }
}
</style>
