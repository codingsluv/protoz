<script setup>
import HeaderComponent from './components/HeaderComponent.vue';
import TheWelcome from './components/TheWelcome.vue';

     
</script>

<template>
  <header>
    <img alt="Logo" class="logo" src="./assets/image.jpeg" width="150" height="125" />
    <HeaderComponent />
  </header>

  <main>
    <TheWelcome />
  </main>
</template>

<style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
  max-width: 150px;
  width: 100%;
  height: auto;
  transition: filter 0.3s ease-in-out;
}

.name {
  font-size: 2rem;
  margin-bottom: 0.5rem;
  text-decoration: underline;
}



@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
