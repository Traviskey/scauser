<script setup>
import LayoutNav from '@/views/Layout/component/LayoutNav.vue'
import LayoutHeader from '@/views/Layout/component/LayoutHeader.vue'
import LayoutFooter from '@/views/Layout/component/LayoutFooter.vue'
import LayoutFixed from "@/views/Layout/component/LayoutFixed.vue"
</script>

<template>
  <LayoutFixed />
  <LayoutNav />
  <LayoutHeader />
  <RouterView />
  <LayoutFooter />
</template>