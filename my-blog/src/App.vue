<template>
  <div id="app">
    <app-header></app-header>
    <router-view></router-view>
    <app-foolter></app-foolter>
  </div>
</template>

<script>
import Header from './components/include/header'
import Footer from './components/include/footer'

export default {
  name: 'App',
  components: {
    'app-header': Header,
    'app-foolter': Footer
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css?family=Roboto:300,400,500,700&display=swap');

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 0px;
  margin-bottom: 0px;
}
.card {
  vertical-align: middle;
}
</style>
