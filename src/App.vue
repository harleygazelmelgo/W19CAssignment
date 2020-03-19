<template>
  <div id="app">
    <Button />
    <TweetList :TweetList="tweets"/>

  </div>
</template>

<script>
import Button from './components/Button.vue'
import TweetList from './components/TweetList.vue'

export default {
  name: 'App',
  components: {
    Button,
    TweetList,

  },
  data() {
    return {
      tweets: [
                {
                  author: "Pope Francis",
                  content: "God's mercy is our liberation and our happiness. We need to forgive, because we ourselves need to be forgiven. #GeneralAudience #Beatitudes"
                },
                  
                {
                  author: "Dalai Lama",
                  content: "Young children don’t care about differences of nationality, faith or race. So long as their companions smile, they play together happily. It seems it’s only as we grow up, in the course of education, that focussing on secondary differences between people creates trouble."
                },

                {
                  author: "Eckhart Tolle",
                  content: "If you had not suffered as you have, there would be no depth to you as a human being, no humility, no compassion. "
                },

                {
                  author: "Law of Attraction",
                  content: "Don't give up just because things are hard. Things are always hard before they get better. Keep your faith alive."
                },

                {
                  author: "Ellen DeGeneres",
                  content: "This tweet is for all the healthcare workers, emergency workers, grocery store workers and more who are doing so much to help us through. We see you and we love you."
                },
                  
                {
                  author: "Daily Zen ",
                  content: "Amidst the doom and gloom atmosphere right now, I see so much to be thankful for— people helping and protecting one another, cooperating and putting aside their differences to solve a common problem. It's hard to be cynical when you honestly recognize our shared perseverance."
                },

                {
                  author: "The Power of Silence",
                  content: "Nourish your body with healthy food, and exercise. Nourish your mind with good literature, art, and company. Nourish your spirit with silence, stillness, and prayer."
                },

                {
                  author: "Barack Obama",
                  content: "We owe a profound debt of gratitude to all our health professionals and everybody who’ll be on the front lines of this pandemic for a long while. They’re giving everything. May we all model our own behavior on their selflessness and sacrifice as we help each other through this.."
                }

              ],
    }
  },
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

body {
  background-color: #009FB7;
}

</style>

