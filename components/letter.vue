<template>
    <v-container>
        <v-card class="mt-5" v-for="item in letters">
                <v-card-title>{{item.name}}</v-card-title>
                <v-card-text>{{ item.description }}</v-card-text>
                <v-spacer/>
          <div class="parent-btn">
                <v-btn>
                     <v-card-text>Удалить</v-card-text>
                </v-btn>
                <v-btn>
                    <v-card-text>Посмотреть</v-card-text>
                </v-btn>
          </div>
        </v-card>
    </v-container>
</template>
<script>
    export default {
        props: {
            letters: {
                type: Array,
                required: true
            }
        },
        data: {

        }
    }
</script>
<style lang="scss" scoped>
    .v-btn{
      background-color: black !important;
      border-radius: 10px !important;
  }
    .v-card{
      display: flex !important;
      flex-direction: column;
    }
      .v-card__text{
        color: white;
      }
    .parent-btn{
      display: flex;
      flex-direction: row;
      align-self: flex-end;
      .v-btn{
        margin: 10px;
      }
    }

</style>
