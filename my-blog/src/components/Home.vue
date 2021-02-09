<template>
    <div id="content">
        <div class="container-grid">
            <h1 style="text-align:left">{{ msg }}</h1>
            <div>
                <div v-for="item in articles" v-bind:key="item.id">
                    <h3>2020-xx-xx｜{{ item.title }}</h3>
                    <!-- <img></img> -->
                    <div>{{ item.subContent }}</div>
                </div>
            </div>
        </div>
        <aside class="aside">
            <div>關於凱</div>
        </aside>
    </div>
</template>

<script>
export default {
  name: 'Home',
  data () {
    return {
      msg: 'Welcome to Kai\'s Blog',
      articles: [
        {id: 0, title: 'article 1', subContent: 'content 1'},
        {id: 1, title: 'article 2', subContent: 'content 2'},
        {id: 2, title: 'article 3', subContent: 'content 3'},
        {id: 3, title: 'article 4', subContent: 'content 4'}
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
