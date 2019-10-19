<template>
    <section>
        <b-field label="Recommended Sun Hours per Day">
            <b-slider type="is-warning" max=24 v-model="value"></b-slider>
        </b-field>
    </section>
</template>

<script>
    export default {
        data() {
            return {
                value: 5
            }
        }
    }
</script>

<style scoped>

</style>