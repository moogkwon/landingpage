<template>
  <v-app>
    <core-app-bar />

    <core-drawer />

    <core-view />

  </v-app>
</template>

<script>
  export default {
    name: 'App',

    components: {
      CoreDrawer: () => import('@/components/core/Drawer'),
      CoreAppBar: () => import('@/components/core/AppBar'),
      CoreView: () => import('@/components/core/View'),
    },
  }
</script>
