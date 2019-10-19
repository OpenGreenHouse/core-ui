<template>

    <b-field label="Name">
        <b-input v-model="name"></b-input>
    </b-field>
</template>

<script>
    export default {
        name: "PlantNameConfigurator",
        data() {
            return {
                name: "What's the name of your plant?"
            }
        }
    }
</script>

<style scoped>

</style>