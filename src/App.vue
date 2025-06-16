<script setup>
import { RouterLink, RouterView } from 'vue-router'
import LoadingScreen from './components/LoadingScreen.vue';
import OkeyCookiesModal from './components/OkeyCookiesModal.vue';
import { ref } from 'vue';

const loading = ref({
  show: true
})

// document.addEventListener(
//   "DOMContentLoaded",
//   () => {
setTimeout(() => {
  loading.value.show = false;
}, 1000)
//   }
// )


const cookies = ref({
  OK: false,
  terms: "",
  fullnote: "",
  notice: `
  
# THIS IS SYSTEM OF MARKDOWN!

Markdown is a lightweight markup language that you can use to add formatting elements to plaintext text documents. Created by John Gruber in 2004, Markdown is now one of the world’s most popular markup languages.
Using Markdown is different than using a WYSIWYG editor. In an application like Microsoft Word, you click buttons to format words and phrases, and the changes are visible immediately. Markdown isn’t like that. When you create a Markdown-formatted file, you add Markdown syntax to the text to indicate which words and phrases should look different.
For example, to denote a heading, you add a number sign before it (e.g., # Heading One). Or to make a phrase bold, you add two asterisks before and after it (e.g., **this text is bold**). It may take a while to get used to seeing Markdown syntax in your text, especially if you’re accustomed to WYSIWYG applications. The screenshot below shows a Markdown file displayed in the Visual Studio Code text editor.
  
### Links to my actions  
> Shordcuts to my work across the internet

---

### More about

| Contact ways | github supervision site | personal entry www |
| --- | --- | --- |
| EMAIL: __sett@sarverott.com__ | GITHUB SITE: https://sarverott.github.io/ | WWW: https://sarverott.com/ |

---
  
  `
})
</script>

<template>
  <LoadingScreen :show="loading.show"></LoadingScreen>
  <OkeyCookiesModal :cookies-required-notice="cookies.notice" :okidoki-flag="cookies.OK"
    :terms-and-policies-link="cookies.terms" :cookies-full-agreement-link="cookies.fullnote"
    @approval="() => { cookies.OK = true }">
  </OkeyCookiesModal>
  <header>
    <img alt="Vue logo" class="logo" src="@/assets/redscope-tech-logo.png" width="125" height="125" />

    <div class="wrapper">

      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav>
    </div>
  </header>

  <RouterView />
</template>

<style scoped></style>
