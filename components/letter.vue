<template>
    <div>
        <v-card class="mt-5" v-for="letter in letters">
                <v-card-title>{{letter.name}}</v-card-title>
                <v-card-text>{{ letter.description }}</v-card-text>
                <v-spacer/>
                <v-btn>
                     <v-icon>qwe</v-icon>
                </v-btn>
                <v-btn>
                    <v-icon>qe</v-icon>
                </v-btn>
        </v-card>
    </div>
</template>
<script>
    export default {
        props: {
            letters: {
                type: Array,
                required: true
            }
        }
    }
</script>
<style scoped></style>