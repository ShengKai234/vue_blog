<template>
  <div id="app">
    <app-header></app-header>
    <app-menu></app-menu>
    <router-view></router-view>
    <app-foolter></app-foolter>
  </div>
</template>

<script>
import Header from './components/include/header'
import Footer from './components/include/footer'
import Menu from './components/include/menu'

export default {
  name: 'App',
  components: {
    'app-header': Header,
    'app-foolter': Footer,
    'app-menu': Menu
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
}
.card {
  vertical-align: middle;
}
</style>
