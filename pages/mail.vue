<template>
    <div>
        <h2>Mail</h2>
        <v-card>
            <letterV :letters="letters"/>
          </v-card>
    </div>
</template>
<script>
import letterV from "../components/letter.vue";
    export default{
        components: {
            letterV
        },
        data: {
            letters: [
                {id: 'id', name:'name', description: 'desc'},
                {id: 'id', name:'name', description: 'desc'},
                {id: 'id', name:'name', description: 'desc'},
            ]
}
}
</script>
<style scoped>

</style>