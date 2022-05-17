<template>
  <v-container>
    <v-row no-gutters>
      <v-col
        v-for="item in Allproduct"
        :key="item.id_product"
        cols="12"
        sm="6"
        md="8"
      >
        <v-card class="pa-2" outlined tile>
          <v-img :src="item.image_path" />
        </v-card>
      </v-col>
      <v-col cols="6" md="4">
        <v-card class="pa-2" outlined tile>
          <h3>{{ item.name }}</h3>
          <h5>{{ item.price }}</h5>
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
    Allproduct: graphql`
      query MyQuery($id_product: uuid!) {
        Allproduct_by_pk(id_product: $id_product) {
          id_product
          image_path
          name
          price
        }
      }
    `,
  },
}
</script>
