<template>
  <div id="app" class="min-h-screen flex flex-col items-center justify-center bg-blue-darkest p-8">
    <div class="w-sm max-w-sm bg-white p-8 sm:py-16">
      <h1 class="text-3xl md:text-4xl mb-4">Stage Viewer</h1>
      <p class="mb-2 text-left">Stage Viewer helps you visualize your church's stage layout.</p>
      <p class="mb-2 text-left">Integrate with Planning Center to organize your band and worship team while providing clarity to your Band, Front of House and Media teams.</p>
      <a href='#learn-more' class="m-2 inline-block" @click.once="learnMoreOpen = true" v-if="!learnMoreOpen">Learn More</a>
      <div id="learn-more" class="mt-8">
        <div v-if="learnMoreOpen" class="mb-8 text-left text-sm">
          <hr class="bg-grey-light h-1 w-full my-8">
          <p>Stage Viewer aims to fill the gap for a few common problems that churches face every week. Knowing who is on stage and where seems like a simple problem to solve. Unfortunately, we struggle with this every week!</p>
          <p>Imagine an audio engineer is a back room mixing the worship service in real time on a separate console. Without a live video feed, they can't see who is on stage and what mic they are using. Singers can change every week, making it hard to label the board with static names.</p>
          <p>Worship teams with a large pools of singers often swap mics on a weekly basis. Wouldn't it be great if they could see which mic and pack they were assigned to on a screen above the mic cabinet?</p>
          <p>Stage Viewer can help with all of these scenarios and more, by allowing you to create a virtual representation of your stage layout every week, accessbile online with a simple shareable URL.</p>
        </div>
      </div>
      <h2 class="mb-4">Interested?</h2>
      <SignUp/>
      <a class="inline-block mt-8" href="#feedback" @click="submitFeedback">Got Feedback?</a>
    </div>
  </div>
</template>

<script>
import SignUp from './components/SignUp.vue'

export default {
  name: 'app',
  components: {
    SignUp
  },
  data: function(){
    return {
      learnMoreOpen: false
    }
  },
  methods: {
    submitFeedback: function(){
      window.open('mailto:daron' + 'spence@' + 'gmail.com?subject=Stage Viewer Feedback');
    }
  }
}
</script>

<style>
#app {
  background-image: url('./assets/band.jpg');
  background-size: cover;
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#learn-more p {
  margin-bottom: 1rem;
}

a {
  color: #38A89D;
}
</style>
