<script setup>
import WelcomeItem from './WelcomeItem.vue'

</script>

<template>
    <div class="card-timeline">
        <WelcomeItem>
            <template #heading>TSEREMOONIA</template>
            Vana-Nigula, Praakli, 
            <br> 
            Saaremaa
            <template #heading2>15:00</template>
        </WelcomeItem>
        <WelcomeItem>
            <template #heading>PULMAPIDU</template>
            <a href="https://sorwespa.com/sorwekook/">Sörweköök</a>, Läätsa küla, 
            <br>
            Saaremaa
            <template #heading2>17:00</template>
        </WelcomeItem>
    </div>
</template>

<style scoped>
.card-timeline {
  display: grid;
  padding-top: 2rem;
  padding-left: 2rem;
  padding-right: 2rem;
  justify-content: center;
  background-color: rgba(254, 254, 250, 1);
  position: relative;
  z-index: 1;
}

@media (min-width: 1024px) {
    .card-timeline {
        display: flex;
        justify-content: space-evenly;
        align-items: center;
        min-height: 300px;
    }

}
</style>