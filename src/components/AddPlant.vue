<template>
    <div>
        <button v-on:click="startConfigurationProcess">Add my first plant.</button>

        <div class="shadow-lg" v-if="inConfiguration">
            <PlantNameConfigurator/>
            <PlantSunHourConfigurator/>
        </div>
    </div>
</template>

<script>
    import PlantNameConfigurator from './PlantNameConfigurator.vue'
    import PlantSunHourConfigurator from './PlantSunHourConfigurator.vue'

    export default {
        name: "AddPlant",
        components: {
            PlantSunHourConfigurator,
            PlantNameConfigurator
        },
        data: () => {
            return {
                inConfiguration: false
            }
        },
        methods: {
            startConfigurationProcess: function () {
                this.inConfiguration = true;
            }
        }
    }
</script>

<style scoped>

</style>