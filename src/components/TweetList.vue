<template>
    <div class="tweet-container cards">
        <Tweet class="" v-for="(tweet,index) in tweets" :key="index" :tweetData="tweet"/>
    </div>
</template>

<script>
import Tweet from './Tweet.vue'
    export default {
        name: "TweetList",
        components: {
            Tweet,
        },
        data(){
            return {
                tweets: [
                    {
                        author: "Meynard",
                        content: "My first Tweet"
                    },
                    {
                        author: "Bob",
                        content: "Hello tweeter"
                    },
                    {
                        author: "Jane",
                        content: "Hello World"
                    },
                    {
                        author: "Peter",
                        content: "Hi everyone!"
                    },
                    {
                        author: "John",
                        content: "Something interesting"
                    },
                ],
            };
        },
    }    
</script>

<style scoped>
    .tweet-container{
        display: grid;
        gap: 10px;
        width: 90vw;
        height: 90vh;
        border: 1px solid black;
    }
    .cards{
        grid-template-columns:repeat( auto-fill, minmax(250px, 1fr) );
        text-overflow: ellipsis;
    }
    .list{
        grid-template-columns: 1fr;
    }
</style>