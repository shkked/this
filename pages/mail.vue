<template>
    <v-container>
        <h2>Mail</h2>
      <div>
            <letterV :letters="letters"/>
      </div>
    </v-container>
</template>
<script>
import letterV from "../components/letter.vue";
    export default{
        components: {
            letterV
        },
        data: function () {
            return {
              letters: [
                {id: '1', name:'Письмо от мамы', description: 'Купи белый хлеб'},
                {id: '2', name:'Письмо от бабушки', description: 'Ты когда домой придешь?'},
                {id: '3', name:'Письмо от Печкина', description: 'Не сиди на печи'},
              ]
            }

}
}
</script>
<style scoped>

</style>
