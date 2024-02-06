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
    <TheWelcome />
  </main>
</template>

<style scoped>
header {
  display: flex;
  width: 100%;
  height: 100%;
  padding: 2rem;
  aspect-ratio: 16/9;
}

main {
  padding: 2rem;
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
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
