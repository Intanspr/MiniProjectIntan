<template>
    <v-app-bar
      color="deep-black"
      dense
      dark
      fixed
      height="50%"
    >

      <v-toolbar-title>
        <v-img  src="https://i.postimg.cc/KjmNqZKJ/1625492037799-1.png" max-width="120" max-height="120"/>
      </v-toolbar-title>

      
  <v-row>
    <v-btn text>
      Home
    </v-btn>
    <v-btn
      text>
      Shop
    </v-btn>
    <v-btn
      text>
      About
    </v-btn>
   
  </v-row>

    
      <v-spacer></v-spacer>

      <v-btn icon>
        <v-icon>mdi-account</v-icon>
      </v-btn>

      <v-btn icon>
        <v-icon>mdi-heart</v-icon>
      </v-btn>

      <v-btn icon>
        <v-icon>mdi-magnify</v-icon>
      </v-btn>

      <v-menu
        left
        bottom
      >
    
          <v-btn
            icon
            v-bind="attrs"
            v-on="on"
          >
            <v-icon>mdi-dots-vertical</v-icon>
          </v-btn>


        <v-list>
          <v-list-item
            v-for="n in 5"
            :key="n"
            @click="() => {}"
          >
            <v-list-item-title>Option {{ n }}</v-list-item-title>
          </v-list-item>
        </v-list>
      </v-menu>
    </v-app-bar>
</template>