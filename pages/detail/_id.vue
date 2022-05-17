<template>
  <v-container style="margin-top: 50px">
    <v-row no-gutters>
      <v-col cols="6">
        <v-card class="pa-2" outlined tile>
          <v-img :src="Allproduct_by_pk.image_path" />
        </v-card>
      </v-col>
      <v-col cols="6">
        <v-card class="pa-2" outlined tile>
          <h3>{{ Allproduct_by_pk.name }}</h3>
          <h5>{{ Allproduct_by_pk.price }}</h5>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
import graphql from 'graphql-tag'
export default {
  name: 'ProductPage',
  apollo: {
    Allproduct_by_pk: {
      query: graphql`
        query MyQuery($id_product: uuid!) {
          Allproduct_by_pk(id_product: $id_product) {
            id_product
            image_path
            name
            price
          }
        }
      `,
      variables() {
        return {
          id_product: this.$route.params.id,
        }
      },
    },
  },
}
</script>
