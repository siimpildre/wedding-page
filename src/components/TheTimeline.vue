<script setup>
import WelcomeItem from './WelcomeItem.vue'
import IconItemRsvp from './IconItemRsvp.vue';
import IconRings from './icons/IconRings.vue';
import IconGlasses from './icons/IconGlasses.vue'

</script>

<template>
    <div>
        <h3>
            OOTAME TEID PULMA!
        </h3>
    </div>

    <div class="card-timeline">
        <div>
            <IconItemRsvp>
                <template #icon>
                    <IconRings />
                </template>
            </IconItemRsvp>
            <WelcomeItem>
                <template #heading>TSEREMOONIA</template>
                <a href="https://www.google.com/maps/place/Vana-Nigula,+Praakli,+93860+Saare+maakond/@58.2618381,22.577525,16.63z/data=!4m6!3m5!1s0x46f27278489f2193:0xbad931137cba7818!8m2!3d58.2605525!4d22.5800854!16s%2Fg%2F11c87jbc86?entry=ttu">
                    Vana-Nigula</a>, Praakli, 
                <br> 
                Saaremaa
                <template #heading2>15:00</template>
            </WelcomeItem>
        </div>
        <div>
            <IconItemRsvp>
                <template #icon>
                    <IconGlasses />
                </template>
            </IconItemRsvp>
            <WelcomeItem>
                <template #heading>PULMAPIDU</template>
                <a href="https://sorwespa.com/sorwekook/">Sörweköök</a>, Läätsa küla, 
                <br>
                Saaremaa
                <template #heading2>17:00</template>
            </WelcomeItem>
        </div>
    </div>
</template>

<style scoped>
a {
    color: black;
}

h3 {
  font-size: 1.2rem;
  position: relative;
  padding: 0.5rem;
  text-align: center;
  background-color: rgba(227, 218, 201, 0.8);
}

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

    h3 {
        display: none;
    }

    .card-timeline {
        display: flex;
        justify-content: space-evenly;
        align-items: center;
        min-height: 300px;
    }

}
</style>