<template >
<div class="background">
  <v-container>
    <base-card class="background">
        <v-row
          class="fill-height pa-3"
          align="center"
        >
          <v-col
            cols="7"
          >
            <!-- md="7"
            offset-md="1" -->

            <h1 style="color:white;" class="display-3 font-weight-light">
              Invest in US Stocks with Zero Commission
            </h1>

            <div style="color:white;" class="subheading text-uppercase pl-2 mb-4">
              Manage your portfolio with your local currency.
              Our commission-free trading in US stocks is coming soon.
            </div>

          <v-row>
            <v-col
              cols="5"
            >
                    <v-img
                      :src="require('@/assets/articles/appstorewhite.png')"
                      width="100%"
                    >
                    </v-img>
            </v-col>

            <v-col
              cols="5"
            >
                    <v-img
                      :src="require('@/assets/articles/playstorewhite.png')"
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
              :src="require('@/assets/articles/iphonebuffett.png')"
              width="50%"
            >
            </v-img>
            
          </v-col>
        </v-row>
    </base-card>
  </v-container>
</div>
</template>

<script>
  export default {
    name: 'HomeBanner',
  }
</script>

<style lang="scss" scoped>
.background {
  background: #009E73;
}
</style>
