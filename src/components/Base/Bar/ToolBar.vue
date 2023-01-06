<template>
  <v-container class="fill-height w-75">
    <v-row class="h-100">
      <v-col clos="3" class="fill-height d-flex align-center">
        <v-img src="@/assets/logo-text.png" class="h-35" />
      </v-col>
      <v-col cols="6" class="fill-height d-flex align-center">
        <search-bar />
      </v-col>
      <v-col cols="3" class="fill-height d-flex align-center">
        <cart />
        <user />
      </v-col>
    </v-row>
  </v-container>
</template>

<script lang="ts" setup>
  import SearchBar from './SearchBar.vue';
  import Cart from '../Button/Cart.vue';
  import User from '../Button/User.vue';
</script>

<style scoped>
  .h-35 {
    height: 35%;
  }
</style>
