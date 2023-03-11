<template>
    <div>
      <v-app-bar
        color="deep-purple accent-4"
        dense
        dark
      >
      
      <v-row class="d-flex justify-center">
        <nuxt-link class="text" exact to="/">Главная</nuxt-link>
        <nuxt-link class="text" exact to="/mail"> Письма</nuxt-link>
        <nuxt-link class="text" exact to="/about-us"> О нас</nuxt-link>
      </v-row>
  
        <v-spacer/>
  
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
          <template v-slot:activator="{ on, attrs }">
            <v-btn
              icon
              v-bind="attrs"
              v-on="on"
            >
              <v-icon>mdi-dots-vertical</v-icon>
            </v-btn>
          </template>
  
          <v-list>
            <v-list-item
              v-for="item in 5"
              :key="item"
              @click="() => {}"
            >
              <v-list-item-title>Option {{ item }}</v-list-item-title>
            </v-list-item>
          </v-list>
        </v-menu>
      </v-app-bar>
    </div>
  </template>

<script>
    export default{

    }
</script>

<style scoped>
  .nuxt-link-active{
    color: green;
  }
  .text{
    color: white;
    text-decoration: none;
    margin-left: 20px !important;
  }
</style>