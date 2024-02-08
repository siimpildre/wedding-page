<script setup>
</script>

<template>
  <div class="greetings">
    <h1 class="stalemate">
      Gedli & Siim
    </h1>
    <h3>
      27.07.2024
    </h3>
  </div>
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.5rem;
  position: relative;
  top: 1rem;
}

h3 {
  font-size: 1rem;
  position: relative;
  top: -0.5rem;
}

.stalemate {
  font-family: 'Stalemate';
}

.greetings h1,
.greetings h3 {
  text-align: center;
}

@media (min-width: 1024px) {
  h1 {
  font-weight: 500;
  font-size: 5rem;
  top: 1rem
}

h3 {
  font-size: 2rem;
  position: relative;
  top: -2rem;
}
  .greetings h1,
  
  .greetings h3 {
    text-align: center;
  }
}
</style>
