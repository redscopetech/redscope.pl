<script setup>

import { ref } from 'vue';

const cookies = {
    OKIDOKI: false,

}

function approval() {
    cookies.OKIDOKI = true;
}

</script>

<template>

    <div class="modal is-active" v-if="!cookies.OKIDOKI">
        <div class="modal-background"></div>
        <div class="modal-card">
            <header class="modal-card-head">
                <p class="modal-card-title">Modal title</p>
                <button class="delete" aria-label="close" @click="approval()"></button>
            </header>
            <section class="modal-card-body">
                dddddddddddddd
            </section>
            <footer class="modal-card-foot">
                <div class="buttons">
                    <button class="button is-success" @click="approval()">Save changes</button>
                    <button class="button" @click="approval()">Cancel</button>
                </div>
            </footer>
        </div>
    </div>

</template>

<style lang="css" scoped></style>