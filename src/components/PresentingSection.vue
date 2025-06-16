<script setup>
//import SliderRevealer from './SliderRevealer.vue';
import { onMounted, onUnmounted } from 'vue';
import Particles from 'particlesjs'

onMounted(() => {
    Particles.init({
        selector: '#backgroundImpresionCanvas',
        connectParticles: true,
        //maxParticles: (1000<(window.innerWidth+window.innerHeight)/2)?420:100
        maxParticles: 123
    });
})

on

</script>

<template>
</template>
<style lang="css" scoped></style>