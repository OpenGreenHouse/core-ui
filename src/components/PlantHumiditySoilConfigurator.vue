<template>
    <section>
        <b-field label="Relative Humidity in Soil">
            <b-slider max=100 v-model="value"></b-slider>
        </b-field>
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