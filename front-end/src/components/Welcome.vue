<script setup>
defineProps({
  name: {
    type: String,
    required: true,
  },
  aboutMe: {
    type: String,
    required: true,
  },
})
</script>

<template>
  <div class="greetings">
    <h2>Hello! 😊 My name is:</h2>
    <h1 class="green">{{ name }}</h1>
    <h2 class="green">{{ aboutMe }}</h2>
  </div>
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 4rem;
  position: relative;
  top: -10px;
}

.greetings .green + h2 {
  font-size: 2rem;
  position: relative;
  opacity: 80%;
  top: -10px;
}

.greetings h1, h2{
  text-align: left;
}

@media (min-width: 1024px) {
}
</style>
