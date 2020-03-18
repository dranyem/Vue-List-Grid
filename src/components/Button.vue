<template>
    <div>
        <p @click="toggleView">Grid/List</p>
    </div>
</template>

<script>
    export default {
        name: "Button",
        methods: {
            toggleView(){
                this.$root.$emit('toggle');
            },
        }
    }
</script>

<style scoped>
    p{
        padding: 5px;
        display: inline-block;
        border: 1px solid black;
    }
</style>