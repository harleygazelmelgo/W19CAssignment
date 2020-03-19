<template>
    <div id="tweet-item">
        <h3>{{ author }}</h3>
        <p>{{ content }}</p>
    </div>

</template>

<script>
    export default {
        name: "Tweet",
        props: {
            author: {
                type: String,
                required: true,
            },
            content: {
                type: String,
                required: true,
            }
    
        },
        
};
</script>

<style scoped>

    #tweet-item {
        width: 100%;
        max-width: 300px;
        margin: 30px auto;
        padding: 0 15px;
        border: 1px solid black;
        border-radius: 15px;
        box-sizing: border-box;
        
    }

    h3 {
        text-align: center;
        color: #D62246;
    }

    p {
        text-align: center;
        color: #FFFACC;
    }

</style>