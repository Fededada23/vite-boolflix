<script>
import { store } from './store';
import AppContent from './components/AppContent.vue';
import AppNav from './components/AppNav.vue';
export default {
  components: {
    AppContent,
    AppNav,
  },
  data() {
    return {
      store,
    }
  },
}
</script>

<template lang="">
  <AppNav />
  <AppContent />
</template>

<style lang="scss">
@use './styles/generals.scss' as *;
::-webkit-scrollbar {
  width: 10px;
  height: 10px;
}
::-webkit-scrollbar-track {
  box-shadow: inset 0 0 5px grey;
  border-radius: 5px;
}

::-webkit-scrollbar-thumb {
  background: red;
  border-radius: 5px;
}
</style>