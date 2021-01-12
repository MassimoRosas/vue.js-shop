<template>
  <div id="app">
    <TheHeader></TheHeader>
    <component :is="page"></component>
  </div>
</template>

<script>
import { eventBus } from './main';

import TheHeader from './components/TheHeader';
import User from './components/features/User/User';
import Admin from './components/features/Admin/Admin';

export default {
  name: 'App',
  components: {
    TheHeader,
    User,
    Admin
  },
  data() {
    return {
      page: eventBus.page
    }
    
  },
  created() {
    eventBus.$on('update:page', (page) => {
      this.page = page;
    })
  }
}
</script>

<style>

</style>
