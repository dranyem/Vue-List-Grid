<template>
    <div id="tweet">
        <h1>{{this.tweetData.author}}</h1>
        <p>{{ this.tweetData.content }}</p>
    </div>
</template>

<script>
    export default {
        name: "Tweet",
        props: {
            tweetData: Object,
        }
        
    }
</script>

<style scoped>
    #tweet{
        display: inline-block;
        border: 1px solid black;
        padding: 5px;
        background-color: lightblue;
        box-shadow: 5px 5px gray;
    }
</style>