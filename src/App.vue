<script>

import AppNav from '/src/components/AppNav.vue';
import AppContent from './components/AppContent.vue';
import AppFooter from './components/AppFooter.vue';

export default {
  components: {
    AppNav,
    AppContent,
    AppFooter

  }
}
</script>

<template>
  <AppNav></AppNav>
  <AppContent></AppContent>
  <AppFooter></AppFooter>
</template>

<style lang="scss">
@use './styles/general.scss' as *;
</style>