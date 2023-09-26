<script setup>
    import Breadcrumb from '@/components/Breadcrumbs.vue'
    import { ref } from 'vue'
    import { TabGroup, TabList, Tab, TabPanels, TabPanel } from '@headlessui/vue'
    let categories = ref(['Timeline', 'About', 'Friends', 'Photos'])
    
</script>
<template>
<div class="container mx-auto">
    <Breadcrumb parentTitle='Calender' subParentTitle='Date Picker' />
    <div class="grid grid-cols-12 gap-5">
    <div class="col-span-6">
        <h2> Start date </h2>
        <div id="app">
  <v-app id="inspire">
    <v-row justify="center">
      <v-date-picker v-model="picker"></v-date-picker>
    </v-row>
  </v-app>
</div>
    </div>
    <div class="col-span-6">
        <h2> End date </h2>
    </div>
    </div>
</div>
</template>