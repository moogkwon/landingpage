<template>
  <base-card >
    <v-img
      :src="require('@/assets/articles/vector.png')"
      class="lighten-2"
      height="500"
      width="100%"
    >
      <v-row
        class="fill-height pa-3"
        align="center"
      >
        <v-col
          cols="7"
        >
          <!-- md="7"
          offset-md="1" -->

          <h1 style="color:black;" class="display-3 font-weight-light">
            Invest in US Stocks with Zero Commission
          </h1>

          <div style="color:black;" class="subheading text-uppercase pl-2 mb-4">
            Start investing in US stocks from $1. 
            Make your money work for you wherever & whenever you are.
          </div>

        <v-row>
          <v-col
            cols="5"
          >
                  <v-img
                    :src="require('@/assets/articles/applestore.png')"
                    class="grey lighten-2"
                    width="100%"
                  >
                  </v-img>
          </v-col>

          <v-col
            cols="5"
          >
                  <v-img
                    :src="require('@/assets/articles/playstore.png')"
                    class="grey lighten-2"
                    width="100%"
                  >
                  </v-img>
          </v-col>
        </v-row>

        </v-col>
        <v-col
          cols="5"
        >

          <v-img
            :src="require('@/assets/articles/iphonex.png')"
            class="grey lighten-2"
            width="50%"
          >
          </v-img>
          
        </v-col>
      </v-row>
    </v-img>
  </base-card>
</template>

<script>
  export default {
    name: 'HomeBanner',
  }
</script>
