<script setup>
    import { RouterLink } from 'vue-router'
</script>

<template>
  <nav>    
    <ul class="nav justify-content-center fixed-top mainNav">
        <li class="nav-item btn">
            <RouterLink to="/">Home</RouterLink>
        </li>
        <li class="nav-item btn">
            <RouterLink to="/Project">Project</RouterLink>
        </li>
        <li class="nav-item btn">
            <RouterLink to="/Contact">Contact</RouterLink>
        </li>
    </ul>
  </nav>
  <!-- <RouterLink to="/">Home</RouterLink>
  <RouterLink to="/about">About</RouterLink> -->
</template>

<style scoped>
.mainNav {
    background-color: hsla(160, 100%, 37%, 1);
}
.nav-item {
    padding: 1.25rem 2rem 1.5rem 2rem;
}
</style>