<script setup>
import HelloQuest from './components/HelloQuest.vue'
import HelloWorld from './components/HelloWorld.vue'
import TheTimeline from './components/TheTimeline.vue'
import TheRsvp from './components/TheRsvp.vue'
import TheExtra from './components/TheExtra.vue'
import ByeQuest from './components/ByeQuest.vue'
import TheTransport from './components/TheTransport.vue'

</script>

<template>
  <header>
    <div class="nav-color">
      <HelloQuest />  
    </div>
    <div class="bg-pic-size">
    <div class="background-pic">
      <HelloWorld />
    </div>
  </div>
  </header>

  <main>
    <div>
      <div>
        <TheTimeline />
      </div>
      <div class="pic">
        <img src="./assets/pictures/Tezza-8603.jpg" alt="holding hands pic" class="pic-hands">
      </div>
    </div>

    <div class="first">
      <TheRsvp />
    </div>

    <div>
      <TheExtra />
    </div>

    <div class="first">
      <TheTransport />
    </div>

  </main>

  <footer>
      <ByeQuest />
  </footer>
</template>

<style scoped>

.nav-color {
  width: 100%;
  background-color: rgba(227, 218, 201, 0.8);
  z-index: 1;
  position: relative;
}

.first{
  background-color: rgba(245, 241, 237, 1);
}

.bg-pic-size {
  width: 100%;
}

.background-pic {
  display: flex;
  width: 100%;
  height: auto;
  aspect-ratio: 16/10;
  position: relative;
  justify-content: center;
  align-items: center;
  background-repeat: no-repeat;
  background-size: cover;
  overflow: hidden;
}
.background-pic::before {
  background-image: url("src/assets/pictures/Tezza-9003.JPG");
	background-size: cover;
	position: absolute;
	right: 0px;
	bottom: 0px;
	left: 0px;
	opacity: 0.5;
	content: "";
  top: -3rem;
  scale: 1.5;
  overflow: hidden;
}

img  {
  width: 100%;
}
.pic {
  display: flex;
  justify-content: center;
  background-color: rgba(254, 254, 250, 1);
}

@media (min-width: 1024px) {
  
  .pic-hands {
    width: 40%;
    border-top-right-radius: 50rem;
    border-top-left-radius: 50rem;
    position: relative;
    z-index: 2;
  }

  .background-pic::before {
    top: -15rem;
  }

  header {
    display: grid;
    place-items: center;
    aspect-ratio: 15/9;
  }
}
</style>
