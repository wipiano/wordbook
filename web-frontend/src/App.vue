<template>
  <div id="app">
    <Navigation />
    <router-view/>
  </div>
</template>

<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>

<script src="shims-tsx.d.ts"></script>
<script lang="ts">
  import { Component, Vue } from 'vue-property-decorator';
  import Navigation from '@/components/Navigation.vue'; // @ is an alias to /src

  @Component({
    components: {
      Navigation,
    },
  })
  export default class App extends Vue {}
</script>
