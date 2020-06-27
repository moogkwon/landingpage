<template>
  <v-col
    cols="12"
    :md="size === 2 ? 6 : size === 3 ? 4 : undefined"
  >
    <!-- :md="size === 2 ? 6 : size === 3 ? 4 : undefined" -->
    <base-card
      :height="value.prominent ? 450 : 450"
      href="#!"
    >
      <v-img
        v-if="value.hero !== undefined"
        :src="require(`@/assets/articles/${value.hero}`)"
        aspect-ratio="1.3"
        contain
      >
        <v-row
          v-if="!value.prominent"
          class="fill-height text-left ma-12"
        >
          <v-col cols="12">

            <h3 class="text-h3 title font-weight-medium mb-2">
              {{ value.title }}
            </h3>


            <h2 class="text-h5 caption">
              {{ value.author }}
            </h2>

            <h2 class="text-h7 caption">
              {{ value.description }}
            </h2>

          </v-col>

        </v-row>
      </v-img>
    </base-card>
  </v-col>
</template>

<script>
  export default {
    name: 'FeedCard',

    props: {
      size: {
        type: Number,
        required: true,
      },
      value: {
        type: Object,
        default: () => ({}),
      },
    },
  }
</script>

<style>
.v-image__image {
  transition: .3s linear;
}
.title {
  font-size: 100px !important;
}
</style>
