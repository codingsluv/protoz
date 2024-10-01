<script setup>
     let name = "Muhammad Nur"
     let dreamJob = "Backend-Dev"
</script>

<template>
  <header>
    <img alt="Vue logo" class="logo" src="./assets/image.jpeg" width="150" height="125" />

    <div class="wrapper">
      <nav>
        <a href="/">Home</a>
        <a href="/about">About</a>
        <a href="/contact">Contact</a>
      </nav>
      <h1>{{ name }}</h1>
      <p>I aspire to be a {{ dreamJob }}.</p>
    </div>
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
