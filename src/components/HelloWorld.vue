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
  font-size: 4rem;
  position: relative;
  top: 10px;
}

h3 {
  font-size: 1.2rem;
  position: relative;
  top: -10px;
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
  font-size: 7rem;
}

h3 {
  font-size: 3rem;
  position: relative;
}
  .greetings h1,
  
  .greetings h3 {
    text-align: center;
   
  }
}
</style>
