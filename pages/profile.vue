<template>
  <div class="profile">
    <sidebar></sidebar>
    <section>
      <h1>The Profile Page</h1>
    </section>
  </div>
</template>

<script>
//define the sidebar layout in this page
definePageMeta({
  layout: "sidebar",
});
</script>

<style lang="scss" scoped>
.profile {
  display: flex;
}
</style>
