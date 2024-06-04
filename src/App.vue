<script setup>
import { RouterView } from 'vue-router'
import TopNavigation from './components/TopNavigation.vue'
import BottomFooter from './components/BottomFooter.vue'
</script>

<template>
  <TopNavigation></TopNavigation>
  <RouterView />
  <BottomFooter></BottomFooter>
</template>
