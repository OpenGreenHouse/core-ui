<template>
    <section>
        <p>Name: {{name}}</p>
        <p>Sun Hours: {{sunHours}}</p>
        <p>Light Intensity: {{lightIntensity}}</p>
        <p>Soil Humidity: {{soilHumidity}}</p>
    </section>
</template>

<script>
    export default {
        data() {
            return {
                value: 60
            }
        }
    }
</script>

<style scoped>

</style>