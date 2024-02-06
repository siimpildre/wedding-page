<script setup>
import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/TheWelcome.vue'
</script>

<template>
  <header class="wrapper backgroundPic">
    <div>
      <HelloWorld />
    </div>
  </header>

  <main>
    <div class="card first">
      <TheWelcome />
    </div>

    <div class="card sec">
      <TheWelcome />
    </div>

    <div class="card third">
      <TheWelcome />
    </div>
    
  </main>
</template>

<style scoped>
header {
  display: flex;
  width: 100%;
  height: 100%;
  aspect-ratio: 16/10;
}

main {

}

.card {
  display: flex;
  padding: 2rem;
}
.first{
  background-color: rgba(244, 240, 236, 1);
}

.sec {
  background-color: rgba(254, 254, 250, 1);
}

.third {
  background-color: rgba(227, 218, 201, 1);
}

.backgroundPic {
  position: relative;
  justify-content: center;
  align-items: center;
  background-repeat: no-repeat;

}
.backgroundPic::before {
  background-image: url("src/assets/Tezza-8603.jpg");
	background-size: cover;
	position: absolute;
	top: 0px;
	right: 0px;
	bottom: 0px;
	left: 0px;
	opacity: 0.6;
	content: "";
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
    aspect-ratio: 15/9;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
  .card {
    align-items: center;
    min-height: 300px;
  }

}
</style>
