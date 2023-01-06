<template>
  <v-text-field
    :loading="loading"
    color="info"
    class="rounded-pill"
    placeholder="Goods / Cloth"
    density="compact"
    variant="outlined"
    single-line
    hide-details
  />
  <v-btn variant="flat" prepend-icon="mdi-magnify" color="info" class="ml-5">Search</v-btn>
</template>
<script lang="ts" setup>
  import { ref } from 'vue';
  const loading = ref(false);

  //   function searchGoods() {
  //     console.log('search goods');
  //   }
</script>
