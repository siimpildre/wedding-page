<script setup>
import WelcomeItem from './WelcomeItem.vue'
import IconItemRsvp from './IconItemRsvp.vue';
import IconRsvp from './icons/IconRsvp.vue';

</script>

<template>
    <IconItemRsvp>
        <template #icon>
            <IconRsvp />
        </template>
    </IconItemRsvp>
    <WelcomeItem>
        Ootame väga sinuga koos tähistamist!
        <br>
        <br>
        Palun anna oma tulekust või mitte tulekust teada hiljemalt 27. maiks meili või telefoni teel!
    </WelcomeItem>
</template>
