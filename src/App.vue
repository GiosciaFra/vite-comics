<script>

import AppNav from './components/AppNav.vue';
import AppContent from './components/AppContent.vue';
import AppLinks from './components/AppLinks.vue';

export default {
  components: {
    AppNav,
    AppContent,
    AppLinks,

  }
}
</script>

<template>
  <AppNav></AppNav>
  <AppContent></AppContent>
  <AppLinks></AppLinks>
</template>

<style lang="scss">
@use './styles/general.scss' as *;
</style>