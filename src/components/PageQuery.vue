<script>
export default {
  name: "PageQuery",
};
</script>

<template>
  <div class="query">
    <label for="category">Choose category:</label>
    <select name="category" id="category">
      <option value="volvo">Volvo</option>
      <option value="saab">Saab</option>
      <option value="opel">Opel</option>
      <option value="audi">Audi</option>
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
