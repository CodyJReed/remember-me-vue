<template>
  <the-header title="RememberMe" />
  <stored-resources :resources="storedResources" />
</template>

<script>
import StoredResources from './components/resources/StoredResources.vue';
import TheHeader from './components/layouts/TheHeader.vue';
export default {
  components: {
    StoredResources,
    TheHeader
  },
  data() {
    return {
      storedResources: [
        {
          id: 'offical-guide',
          title: 'Offical Guide',
          desc: 'offical vue js docs',
          link: 'vuejs.org'
        },
        {
          id: 'google',
          title: 'google',
          desc: 'learn to google...',
          link: 'google.com'
        }
      ]
    };
  }
};
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@300&display=swap');

* {
  box-sizing: border-box;
}

html {
  font-family: 'Roboto', sans-serif;
}

body {
  margin: 0;
}

h3 {
  text-transform: capitalize;
}
</style>
