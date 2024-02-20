<template>
  <header>
    <ul>
      <li><RouterLink to="/">Home</RouterLink></li>
      <li><RouterLink to="/todo">Todo</RouterLink></li>
    </ul>
  </header>
  <main>
    <RouterView />
  </main>
</template>

<style scoped></style>

<script>
export default {
  data() {}
}
</script>
