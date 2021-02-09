<template>
    <div>
        <!-- <button class="btn btn-danger btn-rounded" v-on:click="login">Sign in!</button> -->
        <h1>{{ msg }}</h1>
        <div>
            <li v-for="item in articles" v-bind:key="item.id">{{ item.title }}</li>
        </div>
    </div>
</template>

<script>
export default {
  name: 'Home',
  data () {
    return {
      msg: 'Welcome to Kai\'s Blog',
      articles: [
        {id: 0, title: 'article 1'},
        {id: 1, title: 'article 2'},
        {id: 2, title: 'article 3'},
        {id: 3, title: 'article 4'}
      ]
    }
  },
  methods: {
    login: function () {
      this.$router.push({path: '/Login'})
    }
  }
}
</script>
