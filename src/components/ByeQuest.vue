<script setup>
</script>

<template>
  <div class="greetings">
    <h3>
      Gedli & Siim
      <br>
      27.07.2024
      <br>
      <br>
      gedlilest@gmail.com, tel. 54518255
      <br>
      spildre@gmail.com, tel. 56630533
    </h3>
  </div>
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.5rem;
  position: relative;
}

h3 {
  font-size: 1rem;
  position: relative;
}

.space-bt {
  display: flex;
  justify-content: space-between;
}

.greetings {
  padding: 1rem;
  background-color: rgba(227, 218, 201, 1);
}

.greetings h1,
.greetings h3 {
  text-align: center;
}

@media (min-width: 1024px) {
  h1 {
  font-weight: 500;
  font-size: 2rem;
}

h3 {
  font-size: 1.2rem;
  position: relative;
}

.greetings {
  background-color: rgba(227, 218, 201, 1);
}
  .greetings h1,
  
  .greetings h3 {
    text-align: center;
  }
}
</style>
