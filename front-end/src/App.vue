<script setup>
import Welcome from './components/Welcome.vue'
import Portfolio from "@/components/Portfolio.vue";
</script>

<template>
  <header>
    <div class="wrapper">
      <Welcome name="Douglas Riese" about-me="I am a second year Computer Systems Technology student at Saskpolytech." />
    </div>
  </header>

  <main>

    <Portfolio>

    </Portfolio>
  </main>
</template>

<style scoped>
header {
  line-height: 1.5;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
    border-bottom: 1px solid var(--color-border);
  }
}
</style>
