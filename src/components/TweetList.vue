<template>
    <div id="tweet-list" :style='{"display" : (isActive? "grid" : "block" )}'>
        <Tweet v-for="tweet in TweetList" :key="tweet.author" :author="tweet.author" :content="tweet.content" />
    </div>
</template>

<script>
import Tweet from "./Tweet.vue";

export default {
    name: "TweetList",
    props: {
        TweetList: Array,
    },

    components: {
        Tweet
    },
    
    data() {
        return {
            isActive: true
        };
    },

    mounted: function() {
        this.$root.$on('NewStyleTweet', this.NewStyleTweet)
    },

    methods: {
        NewStyleTweet: function() {
            this.isActive = !this.isActive;
        }
    },


};
</script>

<style scoped>

    #tweet-list{
        display: grid;
        grid-template-columns: 1fr 1fr 1fr 1fr;
        grid-column-gap: 20px;
        justify-content: center;
        justify-items: center;
        text-align: center;
        
    }

</style>
