<template>
  <v-footer
    padless
  >
    <v-card
      class="flex"
      flat
      tile
    >
      <v-card-title style="color: white">
        <strong >Contact US</strong>
        <hr><hr>
        
        
        
       

        <v-spacer></v-spacer>

        <v-img  src="https://i.postimg.cc/KjmNqZKJ/1625492037799-1.png" max-width="120" max-height="120"/>
        <br>
        <span>FIND US ON</span>
        <v-btn
          v-for="icon in icons"
          :key="icon"
          class="mx-4 pt-4"
          dark
          icon
        >
          <v-icon size="24px">
            {{ icon }}
          </v-icon>
        </v-btn>
      </v-card-title>

      <v-card-text class="py-2 white--text text-center">
      &copy; {{ new Date().getFullYear() }} — <strong>SUNDS.CO</strong>
      </v-card-text>
    </v-card>
  </v-footer>
</template>

<script>
  export default {
    data: () => ({
      icons: [
        'mdi-facebook',
        'mdi-twitter',
        'mdi-linkedin',
        'mdi-instagram',
      ],
    }),
  }
</script>