<template>
  <v-app >
    <div class="landing">
    <NavPage />

    <v-main>
      <v-container>
        <br>
        <br>
         <v-img  src="https://i.postimg.cc/DzLxvb68/Whats-App-Image-2022-04-25-at-22-37-53.jpg"></v-img>

      <NewApp />

      <br /><br />
      <BestSel />
      </v-container>
    </v-main>
    
    
      <FooterPage />
    </div>
  </v-app>
</template>

<script>
export default {
  name: 'DefaultLayout',
  data() {
    return {
      clipped: false,
      drawer: false,
      fixed: false,
      items: [
        {
          title: 'Index',
          to: '/',
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Inspire',
          to: '/inspire',
        },
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: 'Vuetify.js',
    }
  },
}
</script>

<style>
  .landing{
    background-color: white;
  }
</style>
