<script setup>
import IconItem from './IconItem.vue'
import WelcomeItem from './WelcomeItem.vue';
import IconRings from './icons/IconRings.vue'
import IconDaisy from './icons/IconDaisy.vue'
import IconBox from './icons/IconBox.vue'
import IconBaby from './icons/IconBaby.vue'

</script>
<template>
    <div class="card-extra">
        <WelcomeItem>
            <h3>LISAINFO</h3>
        </WelcomeItem>
        <IconItem>
            <template #icon>
                <IconRings />
            </template> 
            Tseremooniale kogunemine algab 15 minutit varem ning leiab aset lageda taeva all.
        </IconItem>
        <IconItem> 
            <template #icon>
                <IconDaisy />
            </template>
            Lilli palume mitte tuua. Nende asemel võib kinkida lotopileti või mõne hea veini.
        </IconItem>
        <IconItem> 
            <template #icon>
                <IconBox />
            </template>
            Kingituse palume mahutada ümbrikusse.
        </IconItem>
        <IconItem> 
            <template #icon>
                <IconBaby />
            </template>
            Pere pisematele palume selleks õhtuks leida hoidja.
        </IconItem>
    </div>
</template>

<style scoped>

.card-extra {
  display: grid;
  padding: 2rem;
  justify-content: center;
  background-color: rgba(254, 254, 250, 1);
  position: relative;
  z-index: 1;
}

</style>