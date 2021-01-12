<template>
  <div id="app">
    <TheHeader></TheHeader>
    <User></User>
    <Admin></Admin>
  </div>
</template>

<script>
import TheHeader from './components/TheHeader';
import User from './components/features/User/User';
import Admin from './components/features/Admin/Admin';

export default {
  name: 'App',
  components: {
    TheHeader,
    User,
    Admin
  }
}
</script>

<style>

</style>
