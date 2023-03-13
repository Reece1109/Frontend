<template>
  <div>
    <NavBarVue></NavBarVue>
    <router-view></router-view>
    <FootercVue></FootercVue>
  </div>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}

</style>
<script>
import NavBarVue from './components/NavBar.vue';
import FootercVue from './components/FooterC.vue';

export default {
  components: {
    NavBarVue,
    FootercVue
  }
}
</script>
