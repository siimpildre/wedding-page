<script setup>
import WelcomeItem from './WelcomeItem.vue'
import IconItemRsvp from './IconItemRsvp.vue';
import IconBus from './icons/IconBus.vue';

</script>

<template>
    <div class="card-rsvp">
        <IconItemRsvp>
            <template #icon>
                <IconBus />
            </template>
        </IconItemRsvp>
        <WelcomeItem>
            Bussile kogunemiskoht on Selveri taguses parklas kell 14:30 ning buss alustab liikumist tseremooniale 14:40. 
            <br>
            <br>
            Öösel teeb buss vajadusel mitu ringi Kuressaarde ning ühe tiiru ka Kärlalt läbi, et kõik pidulised saaksid soovi korral koju. 
        </WelcomeItem>
    </div>
</template>

<style scoped> 

.card-rsvp {
  display: grid;
  padding-top: 2rem;
  padding-left: 2rem;
  padding-right: 2rem;
  justify-content: center;
  position: relative;
  z-index: 1;
}

  @media (min-width: 1024px) {
    .card-rsvp {
        min-height: 300px;
    }

}
</style>