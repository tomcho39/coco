<template>
  <q-layout view="lHh Lpr lFf">
    <q-header elevated>
      <q-toolbar>
        <q-btn flat round dense icon="menu" class="q-mr-sm">
      <q-menu>
        <q-list dense style="min-width: 100px">
          <q-item clickable v-close-popup>
            <q-item-section>홈</q-item-section>
          </q-item>
          <q-item clickable v-close-popup>
            <q-item-section>최신 코코</q-item-section>
          </q-item>
          <q-item clickable v-close-popup>
            <q-item-section>모든 코코</q-item-section>
          </q-item>
          <q-item clickable v-close-popup>
            <q-item-section>코코 소식</q-item-section>
          </q-item>
          <q-item clickable v-close-popup>
            <q-item-section>코코타운 소개</q-item-section>
          </q-item>
        </q-list>
      </q-menu>
    </q-btn>
        <q-toolbar-title>
          COCO Town
        </q-toolbar-title>
        <q-btn flat round dense icon="assignment_ind"></q-btn>
      </q-toolbar>
    </q-header>
    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>
import { defineComponent, ref } from 'vue'

export default defineComponent({
  name: 'MainLayout',
  setup () {
    const leftDrawerOpen = ref(false)
    return {
      leftDrawerOpen
    }
  }
})
</script>
