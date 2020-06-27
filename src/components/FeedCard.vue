<template>
  <v-col
    cols="12"
    :md="size === 2 ? 6 : size === 3 ? 4 : undefined"
  >
    <!-- :md="size === 2 ? 6 : size === 3 ? 4 : undefined" -->
    <base-card
      :height="value.prominent ? 450 : 350"
      href="#!"
    >
      <v-img
        v-if="value.hero !== undefined"
        :src="require(`@/assets/articles/${value.hero}`)"
        height="100%"
      >
        <v-row
          v-if="!value.prominent"
          class="fill-height text-right ma-12"
        >
          <v-col cols="12">

            <h3 class="title font-weight-bold mb-2">
              {{ value.title }}
            </h3>


            <h2 class="caption">
              {{ value.author }}
            </h2>

            <h2 class="caption">
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
</style>
