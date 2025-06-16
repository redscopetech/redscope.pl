<script setup>
import { onMounted } from 'vue'


// import Reveal from 'reveal.js'
// import Markdown from 'reveal.js/plugin/markdown/markdown.js'
// import Highlight from 'reveal.js/plugin/highlight/highlight.js'
// import 'reveal.js/dist/reveal.css'
// import 'reveal.js/dist/theme/black.css'
// import 'reveal.js/plugin/highlight/monokai.css'

onMounted(() => {
    Reveal.initialize({
        plugins: [Markdown, Highlight],
        markdown: {
            breaks: true,
            gfm: true
        }
    })
})

//import Reveal from 'reveal.js';
// import Markdown from 'reveal.js/plugin/markdown/markdown.esm.js';
// import Highlight from 'reveal.js/plugin/highlight/highlight.esm.js';
// import Notes from 'reveal.js/plugin/notes/notes.esm.js';
// import MathTex from 'reveal.js/plugin/math/math.esm.js';

//
</script>



<template>
    <div class="reveal">
        <div class="slides">

            <section data-markdown>
                <textarea data-template>
## Reveal on Vue.js Template
             made by Lucas Miserez
</textarea>
            </section>
            <section>
                <section data-markdown>
                    <textarea data-template>
            ## This is a vertical slide
            </textarea>
                </section>
                <section>
                    <h2>This is the vertical slide component</h2>
                </section>
            </section>

        </div>
    </div>
</template>

<style scoped></style>