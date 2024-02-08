<script setup>
import HelloQuest from './components/HelloQuest.vue'
import HelloWorld from './components/HelloWorld.vue'
import TheTimeline from './components/TheTimeline.vue'
import TheRsvp from './components/TheRsvp.vue'
import TheExtra from './components/TheExtra.vue'
</script>

<template>
  <header class="wrapper">
    <div class="nav-color">
      <HelloQuest />  
    </div>
    <div class="wrapper background-pic">
      <HelloWorld />
    </div>
  </header>

  <main>
    <div class="card">
      <TheTimeline />
    </div>

    <div class="card first">
      <TheRsvp />
    </div>

    <div class="card">
      <div class="grid">
        <TheExtra />
      </div>

    </div>

  </main>
</template>

<style scoped>

.nav-color {
  width: 100%;
  background-color: rgba(227, 218, 201, 0.8);
  z-index: 1;
  position: relative;
}

.card {
  display: grid;
  padding: 2rem;
  justify-content: center;
  background-color: rgba(254, 254, 250, 1);
  position: relative;
  z-index: 1;
}
.first{
  background-color: rgba(245, 241, 237, 1);
}

.background-pic {
  display: flex;
  width: 100%;
  height: 100%;
  aspect-ratio: 16/10;
  position: relative;
  justify-content: center;
  align-items: center;
  background-repeat: no-repeat;
}
.background-pic::before {
  background-image: url("src/assets/pictures/Tezza-9003.JPG");
	background-size: cover;
	position: absolute;
	top: 0px;
	right: 0px;
	bottom: 0px;
	left: 0px;
	opacity: 0.6;
	content: "";
  top: -3rem;
  transform: scale(1.5)
}

@media (min-width: 1024px) {

  .background-pic::before {
    top: -15rem;
  }

  header {
    display: grid;
    place-items: center;
    aspect-ratio: 15/9;
  }

  .card {
    display: flex;
    justify-content: space-evenly;
    align-items: center;
    min-height: 300px;
    top: -5rem;
  }

  .grid {
    display: grid;
    width: 100%;
    justify-content: center;
  }

}
</style>
