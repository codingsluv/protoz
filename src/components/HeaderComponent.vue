<script setup>
    let name = "Muhammad Nur"
    let dreamJob = "Full-Stack Developer"
    let messageInformation = "I am an enthusiastic person and want to learn a lot of new things."
</script>

<template>
    <div class="wrapper">
      <nav class="nav">
        <a href="/">Home</a>
        <a href="/about">About</a>
        <a href="/contact">Contact</a>
        <a href="/certificate">Certificate</a>
        <a href="/resume">Resume</a>
      </nav>
      <div class="mesage">
            <h1>{{ name }}</h1>
            <h2>{{ dreamJob }}</h2>
            <p>{{ messageInformation }}</p>
        </div>
    </div>
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

.nav {
    display: flex;
    justify-content: space-around;
    margin-bottom: 1rem;
    list-style-type: none;
    padding: 0;
    a {
      color: #333;
      text-decoration: none;
      transition: color 0.3s ease-in-out;
    }
    a:hover {
      color: #000000;
      margin: auto;
      padding: 0.25rem;
    }

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