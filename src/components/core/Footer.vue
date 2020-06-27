<template>
  <v-footer
    class="py-4"
    height="auto"
    style="color:white !important;"
  >
    <v-container class="mx-auto">
      <v-row>
        <v-spacer />

        <base-btn
          class="mr-0"
          square
          title="Go to top"
          @click="$vuetify.goTo(0)"
        >
          <v-icon style="color: white;">mdi-chevron-up</v-icon>
        </base-btn>
      </v-row>
    </v-container>
  </v-footer>
</template>

<script>
  export default {
    name: 'CoreFooter',
  }
</script>

<style lang="scss" scoped>
.button {
  color: green;
}
</style>
