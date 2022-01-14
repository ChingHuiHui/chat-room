<template>
  <div class="h-screen flex flex-col border-4 border-fontech">
    <default-header />
    <content-section />
    <input-section />
  </div>
</template>

<script setup lang="ts">
  import DefaultHeader from './components/DefaultHeader.vue'
  import ContentSection from './components/ContentSection.vue'
  import InputSection from './components/InputSection.vue'
</script>
