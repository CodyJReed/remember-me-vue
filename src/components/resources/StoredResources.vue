<template>
  <ul>
    <LearningResource
      v-for="item in resources"
      :key="item.id"
      :resource="item"
    />
  </ul>
</template>

<script>
import LearningResource from './LearningResource.vue';
export default {
  components: {
    LearningResource
  },
  props: ['resources'],
  mounted() {
    console.log(this.resources);
  }
};
</script>

<style scoped>
ul {
  list-style: none;
  padding: 0;
  margin: auto;
  max-width: 40rem;
}
</style>
