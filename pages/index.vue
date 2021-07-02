<template>
  <div>
    <top-menu />
    <main-baner />
    <sherpa />
    <acting />
    <services />
    <works />
    <tidings />
    <footer-shepa />
  </div>
</template>

<script>
import mainBaner from "~/components/mainBaner.vue";
import sherpa from "~/components/sherpa.vue"
import acting from "~/components/acting.vue"
import services from "~/components/services.vue";
import works from "~/components/works.vue";
import topMenu from "~/components/top_menu.vue";
import tidings from "~/components/tidings.vue"
import footerShepa from "~/components/footer.vue";
export default {
  components: {
    mainBaner,
    sherpa,
    acting,
    services,
    works,
    topMenu,
    tidings,
    footerShepa
  },
};
</script>
