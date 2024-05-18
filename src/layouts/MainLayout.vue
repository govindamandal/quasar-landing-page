<template>
  <q-layout view="lHh Lpr lFf">
    <main-container>
      <q-header class="hyperhire-header">
        <div class="site-name">
          <logo-hyperhire />
        </div>
        <div class="header-menu">
          <div class="header-menu-child">Menu 1</div>
          <div class="header-menu-child">Menu 2</div>
        </div>
        <div class="profile">Profile Button</div>
      </q-header>
      <q-page-container>
        <router-view />
      </q-page-container>
    </main-container>
    <q-footer> Footer </q-footer>
  </q-layout>
</template>
<script setup lang="ts">
import LogoHyperhire from 'src/components/LogoHyperhire.vue';
import MainContainer from './MainContainer.vue';
</script>
