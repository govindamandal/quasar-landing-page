<template>
  <q-layout view="lHh Lpr lFf">
    <main-container>
      <q-header class="hyperhire-header">
        <div class="site-name">
          <logo-hyperhire />
        </div>
        <div class="header-menu">
          <q-btn-dropdown
            class="no-hover header-menu-child"
            label="채용"
            hoverable="false"
          >
            <q-list>
              <q-item clickable v-close-popup>
                <q-item-section class="text-bold cursor-auto">
                  <q-item-label>채용</q-item-label>
                </q-item-section>
              </q-item>
              <q-item clickable v-close-popup>
                <q-item-section>
                  <q-item-label>해외 개발자 원격 채용</q-item-label>
                </q-item-section>
              </q-item>

              <q-item clickable v-close-popup>
                <q-item-section>
                  <q-item-label>외국인 원격 채용 (비개발 직군)</q-item-label>
                </q-item-section>
              </q-item>

              <q-item clickable v-close-popup>
                <q-item-section>
                  <q-item-label>한국어 가능 외국인 채용</q-item-label>
                </q-item-section>
              </q-item>
            </q-list>
          </q-btn-dropdown>
          <div class="header-menu-child">해외 개발자 활용 서비스</div>
        </div>
        <div class="profile">
          <q-btn color="white" text-color="black" label="문의하기" />
        </div>
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
