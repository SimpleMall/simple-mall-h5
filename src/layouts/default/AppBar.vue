<template>
  <v-app-bar height="150" flat>
    <v-container class="fill-height pa-0 ma-0" :fluid="true">
      <navigation-bar />
      <tool-bar />
    </v-container>
  </v-app-bar>
</template>

<script lang="ts" setup>
  import NavigationBar from '@/components/Base/Bar/NavigationBar.vue';
  import ToolBar from '@/components/Base/Bar/ToolBar.vue';
</script>
