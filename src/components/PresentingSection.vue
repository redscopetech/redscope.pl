<script setup>
//import SliderRevealer from './SliderRevealer.vue';

import Particles from 'particles.js'

onMounted(() => {
    Particles.init({
        selector: '#backgroundImpresionCanvas',
        connectParticles: true,
        //maxParticles: (1000<(window.innerWidth+window.innerHeight)/2)?420:100
        maxParticles: 123
    });
})


</script>

<template>
    <section class="hero is-dark is-large">
        <canvas id="backgroundImpresionCanvas"></canvas>
        <div class="hero-head">
            <nav class="navbar">
                <div class="container">
                    <div class="navbar-brand">
                        <a class="navbar-item">
                            <img src="https://bulma.io/assets/images/bulma-type-white.png" alt="Logo" />
                        </a>
                        <span class="navbar-burger" data-target="navbarMenuHeroB">
                            <span></span>
                            <span></span>
                            <span></span>
                            <span></span>
                        </span>
                    </div>
                    <div id="navbarMenuHeroB" class="navbar-menu">
                        <div class="navbar-end">
                            <a class="navbar-item is-active"> Home </a>
                            <a class="navbar-item"> Examples </a>
                            <a class="navbar-item"> Documentation </a>
                            <span class="navbar-item">
                                <a class="button is-info is-inverted">
                                    <span class="icon">
                                        <i class="fab fa-github"></i>
                                    </span>
                                    <span>Download</span>
                                </a>
                            </span>
                        </div>
                    </div>
                </div>
            </nav>
        </div>

        <div class="hero-body">
            <div class="container has-text-centered">
                <p class="title">Title</p>
                <p class="subtitle">Subtitle</p>
            </div>
        </div>

        <div class="hero-foot">
            <nav class="tabs is-boxed is-fullwidth">
                <div class="container">
                    <ul>
                        <li class="is-active">
                            <a>Overview</a>
                        </li>
                        <li>
                            <a>Modifiers</a>
                        </li>
                        <li>
                            <a>Grid</a>
                        </li>
                        <li>
                            <a>Elements</a>
                        </li>
                        <li>
                            <a>Components</a>
                        </li>
                        <li>
                            <a>Layout</a>
                        </li>
                    </ul>
                </div>
            </nav>
        </div>
    </section>

</template>
<style lang="css" scoped>
#backgroundImpresionCanvas {
    position: absolute;
    display: block;
    top: 0;
    left: 0;
    z-index: 0;
}
</style>