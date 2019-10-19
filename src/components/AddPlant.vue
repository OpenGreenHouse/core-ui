<template>
    <div>
        <!--        <button v-on:click="startConfigurationProcess">Add my first plant.</button>-->

        <div class="shadow-lg" v-if="inConfiguration">
            <b-steps>
                <b-step-item v-model="showName" label="Name">
                    <PlantNameConfigurator/>
                </b-step-item>

                <b-step-item v-model="showSunHours" label="Sun Hours" icon="alarm">
                    <PlantSunHourConfigurator/>
                </b-step-item>

                <b-step-item v-model="showLightIntensity" label="Light Intensity" icon="weather-sunny">
                    <PlantLuminousIntensityConfigurator/>
                </b-step-item>

                <b-step-item v-model="showHumidity" label="Humidity" icon="water">
                    <PlantHumiditySoilConfigurator/>
                </b-step-item>
            </b-steps>
        </div>
    </div>
</template>


<script>
    import PlantNameConfigurator from './PlantNameConfigurator.vue'
    import PlantSunHourConfigurator from './PlantSunHourConfigurator.vue'
    import PlantLuminousIntensityConfigurator from './PlantLuminousIntensityConfigurator.vue'
    import PlantHumiditySoilConfigurator from './PlantHumiditySoilConfigurator.vue'

    export default {
        name: "AddPlant",
        components: {
            PlantSunHourConfigurator,
            PlantLuminousIntensityConfigurator,
            PlantHumiditySoilConfigurator,
            PlantNameConfigurator
        },
        data: () => {
            return {
                inConfiguration: true,
                showName: true,
                showSunHours: false,
                showLightIntensity: false,
                showHumidity: false,
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