<template>
  <div>
    <nav>
      <nuxt-link to="/">Home</nuxt-link>
      <nuxt-link to="/about">About</nuxt-link>
      <nuxt-link to="/profile">Profile</nuxt-link>
    </nav>
    <!-- nuxt will go to default vue file before moving forward to other pages -->
    <h1>Hello from Layout (default)</h1>
    <!-- if you want to see other pages insert slot element here -->

    <!-- here nuxt will replace page content -->
    <slot></slot>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

nav {
  a {
    font-size: 1rem;
    display: inline-block;
    padding: 0.5rem;
    border: 1px solid #333;
    margin: 0.25rem 0.5rem;
    text-decoration: none;
    &:hover {
      border-color: #793737;
    }
  }
}
</style>
