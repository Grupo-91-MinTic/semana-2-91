<template>
  <div id="app">
    <services></services>
    <footer-section></footer-section>
  </div>
</template>

<script>

import FooterSection from './components/FooterSection.vue';
import Services from './components/Services.vue';

export default {
  name: 'App',
  components: {
    FooterSection,
    Services
  }
}
</script>

