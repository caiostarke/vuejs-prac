<template>

    <button @click="isActive = 'StepOne'"> Step One</button>
    <button @click="isActive = 'StepTwo'"> Step Two</button>

    <keep-alive>
        <component :is="isActive"></component>
    </keep-alive>

</template>

<script>
    import StepOne from './StepOne.vue';
    import StepTwo from './StepTwo.vue';

    export default {
        components: {
            StepOne,
            StepTwo
        },

        data() {
            return {
                isActive: 'StepOne'
            }
        }
    }

</script>