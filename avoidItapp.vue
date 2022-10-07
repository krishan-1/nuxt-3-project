<template>
  <div>
    <!-- above tag is not like home compnent directly calling it means home is directory and after the component which is welcome or HomeWelcome -->

    <!-- <home-welcome></home-welcome> -->

    <!-- below is direct component-->

    <!-- <counter-btn></counter-btn> -->

    <!-- dynamic component -->

    <!-- without mentioning here about index-it will not-->
    <nuxt-page></nuxt-page>

    <a href="#" @click="view('home')">Home</a>
    <a href="#" @click="view('counter')">Counter</a>

    <Lazyhome-welcome v-if="page == 'home'"></Lazyhome-welcome>
    <Lazycounter-btn v-if="page == 'counter'"></Lazycounter-btn>
  </div>
</template>

<script setup>
const page = ref("home");

function view(name) {
  page.value = name;
}
</script>

<style lang="scss" scoped>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

a {
  font-size: 1rem;
  padding: 0.5rem;
  border: 1px solid #333;
  margin: 0.25rem 0.5rem;
  text-decoration: none;
  &:hover {
    border-color: #793737;
  }
}
</style>
