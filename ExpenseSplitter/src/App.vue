<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
import { useRoute } from 'vue-router';

const route = useRoute();

</script>

<template>
  <header>
    <!-- <img alt="Vue logo" class="logo" src="@/assets/logo.svg" width="125" height="125" /> -->

    <div class="wrapper">
      <nav v-if="!route.meta.hideHeader">
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/splitter">Splitter</RouterLink>
        <!-- <RouterLink to="/about">Login</RouterLink>
        <RouterLink to="/about">Sign Up</RouterLink> -->
      </nav>
      <!-- <nav v-if="route.meta.hideHeader">
        <RouterLink to="/">Groups</RouterLink>
        <RouterLink to="/splitter">Activity</RouterLink>
        <RouterLink to="/about">Profile</RouterLink>
      </nav> -->
      <!-- <HelloWorld msg="Welcome" /> -->
    </div>
  </header>

  <RouterView />
</template>

<style scoped>
header {
  /* display: flex; */
  /* line-height: 1.5; */
  /* max-height: 100vh; */
}

/* .logo {
  display: block;
  margin: 0 auto 2rem;
} */

nav {
  padding: 1rem;
  margin: 1rem;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}
</style>
