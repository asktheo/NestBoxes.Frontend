<script setup>
import { RouterView } from 'vue-router';
import navigation from '@/components/main/navigation.vue';
</script>

<template>
  <div class="container-fluid">
    <navigation></navigation>
    <router-view></router-view>
  </div>
</template>

<style>
@media only screen and (max-width: 1600px) {
  body {
    width: 100%;
  }
}

@media only screen and (min-width: 1600px) {
  body {
    width: 90%;
    margin: auto;
  }
}

.form-check-label {
  font-weight: bolder;
}

a {
    text-decoration: none;
    color: var(--bs-emphasis-color);
}

.btn-outline-secondary {
  border: 1px solid var(--bs-border-color-translucent);
}

.btn-outline-secondary:hover {
  border: 1px solid var(--bs-border-color-translucent);
  background-color: inherit;
  color: inherit;
}

.dropdown-menu {
  --bs-dropdown-link-active-bg: var(--bs-white);
}

.bg-nestbox-light,
.bg-nestbox-light:focus
{
  background-color: #00000010;
}
</style>