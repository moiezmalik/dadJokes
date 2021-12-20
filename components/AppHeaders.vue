<template>
    <nav class="navbar navbar-expand-sm bg-dark navbar-dark">
      <!-- Brand/logo -->
      <a class="navbar-brand" href="#">Dad Jokes</a>

      <!-- Links -->
      <ul class="navbar-nav">
        <li class="nav-item">
            <nuxt-link class="nav-link" to="/">Home</nuxt-link>
        </li>
        <li class="nav-item">
            <nuxt-link class="nav-link" to="/jokes">Jokes</nuxt-link>
        </li>
        <li class="nav-item">
            <nuxt-link class="nav-link" to="/about">About</nuxt-link>
        </li>
      </ul>
    </nav>
</template>

<script>
export default {
  name: "AppHeader",
};
</script>

<style>
</style>