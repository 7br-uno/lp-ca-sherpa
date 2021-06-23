<template>
  <div class="indigo">
    <v-container py-16>
      <v-row class="mb-10">
        <v-col cols="12">
          <div class="d-flex justify-center text-h4 text-uppercase font-weight-bold mb-16 text-center white--text">
            Nosso trabalho de web design
          </div>
        </v-col>
        <v-col md="4" lg="4" sm="6" cols="12" class="d-flex justify-center" v-for="(work, i) in works" :key="i">
          <v-hover>
            <template v-slot:default="{ hover }">
            <div :class="`elevation-${hover ? 16 : 4}`" class="transition-swing card__work">
              <v-icon
                x-large
                color="white"
              >
                {{work.icon}}
              </v-icon>
              <div class="text-body-1 mt-2">
                {{work.title}}
              </div>
            </div>
            </template>
          </v-hover>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>
<script>
export default {
  data: () => {
    return {
      works: [
        {title: "Sites", icon:"mdi-web"},
        {title: "Landing Pages personalizadas", icon:"mdi-page-layout-header"},
        {title: "Blog", icon:"mdi-book-open-page-variant"},
        {title: "Identidade Visual", icon:"mdi-account-supervisor-circle-outline"},
        {title: "Marca", icon:"mdi-head-lightbulb-outline"},
        {title: "Cartões Virtuais", icon:"mdi-card-account-details"},
      ]
    }
  }
}
</script>
export default {
  data: () => {
    return {

    }

<style lang="scss" scoped>
.card__work{
  height: 200px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  text-align: center;
  width: 200px;
  border: 2px solid #fff
}
</style>
