<script setup>
import { RouterLink, RouterView } from "vue-router";
import HelloWorld from "./components/HelloWorld.vue";
import AboutView from "./views/AboutView.vue";
import HomeView from "./views/HomeView.vue";
import NavButton from "./components/NavButton.vue";
</script>

<template>
  <header class="min-h-screen">
    <div>
      <HelloWorld msg="Hi there! 🤯" />
      <nav>
        <NavButton label="Skills" href="#skills" >aa</NavButton>
        <NavButton label="Projects" href="#projects" >aa</NavButton>
      </nav>
    </div>
  </header>
  <main>
    <article id="skills">
      <HomeView />
    </article>
    <article id="projects">
      <AboutView />
    </article>
  </main>
</template>

<style scoped>
header {
  display: flex;
  padding-right: calc(var(--section-gap) / 2);
  max-width: 90%;
  background-color: white;
  align-content: center;
  min-height: 100vh;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
}

main {
    text-align: left;
    width: 100%;
    max-width: 90%;
  }

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: white;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    padding-right: calc(var(--section-gap) / 2);
    max-width: 50%;
    background-color: white;
    place-items: center;
    min-height: 100vh;
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }

  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;
    padding: 1rem 0;
    margin-top: 1rem;
  }

  main {
    text-align: left;
    width: 100%;
    max-width: 50%;
  }

  article {
    margin-top: 1.8rem;
  }
}
</style>
