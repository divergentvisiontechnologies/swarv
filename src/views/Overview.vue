<template>
    <main>
        <h1>Overview</h1>
        <AllRecordings v-bind:audiorecordings="audiorecordings"/>
    </main>
</template>

<script>
import AllRecordings from '../components/AllRecordings.vue'
export default {
    name: 'Overview',
    components: {
        AllRecordings
    },
  data() {
    return {
      audiorecordings: [
        {
          id: 1,
          name: "LaLaLa",
          artists: "Y2K & BBN0$",
          singleAudio: "",
          preface: "Song from Tik Tok",
          lyric: "When i popped off and your girl...",
        },{
          id: 2,
          name: "Why Are You Here?",
          artists: "Machine Gun Kelly",
          singleAudio: "",
          preface: "that really awesome indie song",
          lyric: "I hate that i saw you again last night...",
        },{
          id: 3,
          name: "Revenge",
          artists: "Joyner Lucas",
          singleAudio: "",
          preface: "very rough and straight",
          lyric: "The more that i want, the more that i grind...",
        },
      ]
    }
  }
}
</script>

<style scoped>

</style>