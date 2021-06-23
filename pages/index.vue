<template>
  <div>
    <top-menu />
    <main-baner />
    <services />
    <works />
  </div>
</template>

<script>
import mainBaner from "~/components/mainBaner.vue";
import services from "~/components/services.vue";
import works from "~/components/works.vue";
import topMenu from "~/components/top_menu.vue"
export default {
  components: {
    mainBaner,
    services,
    works,
    topMenu
  },
};
</script>
