<script setup>
import WelcomeItem from './WelcomeItem.vue'
import IconItemRsvp from './IconItemRsvp.vue';
import IconRsvp from './icons/IconRsvp.vue';

</script>

<template>
    <div class="card-rsvp">
        <IconItemRsvp>
            <template #icon>
                <IconRsvp />
            </template>
        </IconItemRsvp>
        <WelcomeItem>
            Ootame väga sinuga koos tähistamist!
            <br>
            <br>
            Palun anna oma tulekust või mitte tulekust teada hiljemalt 27. maiks <a href="google.com">siit!</a>!
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