<template>
  <v-card class="overflow-hidden">
    <v-app-bar
      absolute
      color="grey lighten-5"
      elevate-on-scroll
      scroll-target="#scrolling-techniques-7"
    >
      <v-app-bar-nav-icon></v-app-bar-nav-icon>

      <v-toolbar-title>Title</v-toolbar-title>

      <v-spacer></v-spacer>
    </v-app-bar>
    <v-sheet id="scrolling-techniques-7" class="overflow-y-auto" height="100vh">
      <main-baner />
      <services />
      <works />
    </v-sheet>
  </v-card>
</template>

<script>
import mainBaner from "~/components/mainBaner.vue";
import services from "~/components/services.vue";
import works from "~/components/works.vue";
export default {
  components: {
    mainBaner,
    services,
    works,
  },
};
</script>
