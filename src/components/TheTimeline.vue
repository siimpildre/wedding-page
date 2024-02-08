<script setup>
import WelcomeItem from './WelcomeItem.vue'

</script>

<template>
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
</template>
