<template>
  <footer class="clearAllContainer">
    <span class="clearAllBtn" v-on:click="clearAllItems">Clear All</span>
  </footer>
</template>

<script>
import { mapMutations } from 'vuex';

export default {
  methods: {
    ...mapMutations({
      clearAllItems: 'clearAllItems',
    }),
  },
};
</script>

<style scoped>
.clearAllContainer {
  width: 8.5rem;
  height: 50px;
  line-height: 50px;
  background-color: white;
  border-radius: 5px;
  margin: 0 auto;
}
.clearAllBtn {
  color: #e20303;
  display: block;
}
</style>
