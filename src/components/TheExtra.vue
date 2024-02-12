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
            <h3>LISAINFO</h3>
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
            Pere pisematele palume selleks päevaks leida hoidja.
        </IconItem>
    </div>
</template>

<style scoped>

h3 {
  font-size: 1.1rem;
  font-weight: 500;
  margin-top: 2rem;
  color: var(--color-heading);
  text-align: center;
}

.card-extra {
  display: grid;
  padding: 2rem;
  justify-content: center;
  background-color: rgba(254, 254, 250, 1);
  position: relative;
  z-index: 1;
}


</style>