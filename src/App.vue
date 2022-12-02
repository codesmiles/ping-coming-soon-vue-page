<script lang="js">
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://vuejs.org/api/sfc-script-setup.html#script-setup

import Header from './components/Header.vue';

export default {
components:{ Header }
};
</script>

<template>

  <Header/>

  <p>Subscribe and get notified</p>
  <form>
    <input type="email"
      name="email"
      id="email"
      placeholder="Your email address"
    />
      
    <input type="submit" value="Notify Me" />
  </form>

  <div>&copy; Copyright Ping. All rights reserved.</div>

  <footer>
    <p class="attribution">
      Challenge by
      <a href="https://www.frontendmentor.io?ref=challenge" target="_blank"
        >Frontend Mentor</a
      >. Coded by <a href="#">Your Name Here</a>.
    </p>
  </footer>
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
