<script setup>
import Welcome from './components/Welcome.vue'
import TheWelcome from './components/TheWelcome.vue'
</script>

<template>
  <header>
    <div class="wrapper">
      <Welcome name="Douglas Riese" about-me="I am a second year Computer Systems Technology student at Saskpolytech." />
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
