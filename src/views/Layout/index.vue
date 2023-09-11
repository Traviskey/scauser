<script setup>
import LayoutNav from '@/views/Layout/component/LayoutNav.vue'
import LayoutHeader from '@/views/Layout/component/LayoutHeader.vue'
import LayoutFooter from '@/views/Layout/component/LayoutFooter.vue'
import LayoutFixed from "@/views/Layout/component/LayoutFixed.vue"

import {useCategoryStore} from "@/stores/category";
import {onMounted} from "vue";

const categoryStore = useCategoryStore();

onMounted(() => categoryStore.getCategory())
</script>

<template>
  <LayoutFixed />
  <LayoutNav />
  <LayoutHeader />
  <RouterView />
  <LayoutFooter />
</template>