<script>
import axios from "axios";
import { store } from "../store.js";
import PageQuery from "./main-components/PageQuery.vue";
import CardBox from "./main-components/CardBox.vue";

export default {
  name: "PageMain",
  components: {
    PageQuery,
    CardBox,
  },
  data() {
    return {
      store,
    };
  },
  methods: {
    changeQuery() {
      this.store.characters = [];
      axios
        .get(`https://www.breakingbadapi.com/api/characters`, {
          params: {
            category: this.store.categoryQuery,
          },
        })
        .then((resp) => {
          this.store.characters = resp.data;
        });
    },
  },
  created() {
    this.changeQuery();
  },
};
</script>

<template>
  <PageQuery @search="changeQuery" />
  <div class="card-container">
    <div class="found">
      <h3>Trovati {{ store.characters.length }} sbabbari</h3>
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
