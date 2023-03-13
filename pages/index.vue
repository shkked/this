<template>
  <v-container>
    <h1 >Главная</h1>
      <v-carousel>
        <v-carousel-item
          v-for="(item,i) in items"
          :key="i"
          :src="item.src"
          reverse-transition="fade-transition"
          transition="fade-transition"
        ></v-carousel-item>
      </v-carousel>
  </v-container>
</template>

<script>
export default {
  data: function() {
    return {
      i: 2,
      items: [
        {src: 'item1.jpg'},
        {src: 'item2.png'},
        {src: 'item3.png'},
      ]

    }

  }
}
</script>

<style scoped>
</style>
