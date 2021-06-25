<template>
  <div>
    <top-menu />
    <main-baner />
    <sherpa />
    <acting />
    <services />
    <works />
  </div>
</template>

<script>
import mainBaner from "~/components/mainBaner.vue";
import sherpa from "~/components/sherpa.vue"
import acting from "~/components/acting.vue"
import services from "~/components/services.vue";
import works from "~/components/works.vue";
import topMenu from "~/components/top_menu.vue"
export default {
  components: {
    mainBaner,
    sherpa,
    acting,
    services,
    works,
    topMenu
  },
};
</script>
