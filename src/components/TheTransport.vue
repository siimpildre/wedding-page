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
            Pulmalistele broneeritud buss sõidab nii tseremooniale, peokohta kui ka õhtul tagasi. 
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