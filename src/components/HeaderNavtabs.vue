<script setup>
import { RouterLink } from 'vue-router'
</script>

<template>
    <header>
        <img alt="Vue logo" class="logo" src="@/assets/redscope-tech-logo.png" width="125" height="125" />
        <nav class="tabs is-centered is-boxed">
            <ul>
                <li class="is-active is-danger">
                    <RouterLink to="/">
                        <span class="icon is-small">
                            &#x1F441;
                        </span>
                        <span>Homepage</span>
                    </RouterLink>
                </li>
                <li>
                    <RouterLink to="/about">
                        <span class="icon is-small">
                            &#x001F;
                        </span>
                        <span>More about Us</span>
                    </RouterLink>
                </li>
                <li>
                    <RouterLink to="/">
                        <span class="icon is-small">
                            &#x26E7;
                        </span>
                        <span>Our projects</span>
                    </RouterLink>
                </li>
                <li>
                    <RouterLink to="/">
                        <span class="icon is-small">
                            &#x1F7D9;
                        </span>
                        <span>Contact Us</span>
                    </RouterLink>
                </li>
            </ul>
        </nav>
    </header>
</template>

<style lang="css" scoped>
:root {
    --bulma-tabs-link-active-color: #8f0000;
}
</style>