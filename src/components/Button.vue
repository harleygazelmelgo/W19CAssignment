<template>
    <div id="tweet-toggle">
        <button @click='toggleTweet'>click here!</button>
    </div>
</template>

<script>
    export default {
        methods: {
            toggleTweet: function() {
                this.$root.$emit('NewStyleTweet')
            }
        },
    }
</script>



<style scoped>

    #tweet-toggle {
        display: flex;
        margin-top: 20px;
        justify-content: center;
        align-items: center;
    }

    
</style>