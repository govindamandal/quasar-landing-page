<template>
  <q-layout view="lHh Lpr lFf">
    <main-container>
      <!-- Header -->
      <header-layout />
      <q-page-container>
        <router-view />
      </q-page-container>
    </main-container>
    <footer-layout />
  </q-layout>
</template>
<script setup lang="ts">
import MainContainer from './MainContainer.vue';
import HeaderLayout from './HeaderLayout.vue';
import FooterLayout from './FooterLayout.vue';
</script>
