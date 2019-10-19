<template>
    <section>
        <div class="block">

            <b-field label="Light Intensity">
                <div class="block">
                    <b-radio v-model="radio"
                             name="name"
                             native-value="Low">
                        Low
                    </b-radio>
                    <b-radio v-model="radio"
                             name="name"
                             native-value="Medium">
                        Medium
                    </b-radio>
                    <b-radio v-model="radio"
                             name="name"
                             native-value="High">
                        High
                    </b-radio>
                </div>


            </b-field>
        </div>
    </section>
</template>

<script>
    export default {
        data() {
            return {
                radio: ''
            }
        }
    }
</script>

<style scoped>

</style>