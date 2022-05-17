<template>
  <div class="app">
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
            <v-img src="https://i.postimg.cc/nz0rJDJn/1625492037799-1.png" />
          </v-card>
        </v-col>

        <v-spacer />
        <v-col cols="6" md="4">
          <br /><br />
          <br />
          <v-card class="pa-2" outlined tile>
            <h3>
              Sunds.co adalah sebuah brand lokal dari Cikampek, kab.karawang
            </h3>
            <h3>
              Brand yang berlandaskan tentang kearifan lokal , budaya dan
              kesatuan bangsa , berdiri pada tahun 2020, nama dari brand
              sunds.co di ambil dari SUN SUNDAISME CLOTHING yang artinya adalah
              SUN - MATAHARI , SUNDA - SUKU/RAS , ISME - sufiks pembentuk nomina
              sistem kepercayaan berda-sarkan politik, sosial. Sejauh ini brand
              sunds.co baru masuk pasar online dan belum ada offline outlet ,
              Selain baju sund.co juga memproduksi dan menjual aksesoris seperti
              gelang tangan, walldecor, gantungan kunci dan lain - lain
            </h3>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
    <Young />
  </div>
</template>

<script>
export default {
  name: 'AboutPage',
}
</script>

<style>
.app {
  background-color: black;
}
</style>
