<template>
  <div>
    <main class="user-layout">
      <aside>
        <p>Dashboard</p>
        <p>Settings</p>
      </aside>
      <!-- this will show the content -->
      <section>
        <slot></slot>
      </section>
    </main>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
aside {
  display: flex;
  flex-direction: column;
}
</style>
