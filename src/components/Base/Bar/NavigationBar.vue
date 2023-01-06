<template>
  <v-row class="bg-grey-darken-2 h-25">
    <v-container class="fill-height w-75">
      <v-row>
        <v-col cols="12" class="fill-height d-flex align-center">
          <v-btn
            variant="plain"
            size="x-small"
            v-for="data in links"
            :key="data.title"
            @click="openUrl(data.url)"
            >{{ data.title }}</v-btn
          >
        </v-col>
      </v-row>
    </v-container>
  </v-row>
</template>

<script lang="ts" setup>
  interface NavigationElement {
    title: string;
    url: string;
  }

  const links: NavigationElement[] = [
    {
      title: 'Index',
      url: 'https://github.com/suyuan32',
    },
    {
      title: 'doc',
      url: 'https://doc.ryansu.pro/',
    },
  ];

  function openUrl(url: string) {
    window.location.href = url;
  }
</script>
