<template>
  <div>
    <p>
      <router-link to="/">Index</router-link><br>
      <router-link to="/page1">Go to page 1</router-link><br>
      <router-link to="/page2">Go to page 2</router-link><br>
    </p>
    <router-view></router-view>
  </div>
</template>

<script>
  import VueRouter from 'vue-router'
  import Page1 from './Page1.vue'
  import Page2 from './Page2.vue'

  const routes = [
    { path: '/', redirect: '/page1' },
    { path: '/page1', component: Page1 },
    { path: '/page2', component: Page2 },
  ]

  const router = new VueRouter({
    routes,
    mode: 'history',
  })

  export default {
    router,
  }
</script>
