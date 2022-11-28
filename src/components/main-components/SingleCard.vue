<script>
export default {
  name: "SingleCard",
};
</script>

<template>
  <div class="card">
    <img src="https://www.mrw.it/img/cope/0iwkf4_1609360688.jpg" alt="" />
    <h3>Nome Bomber</h3>
    <p>Visto Dove</p>
    <p>Vivo o morto</p>
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
  p {
    color: darkgray;
  }
}
</style>
