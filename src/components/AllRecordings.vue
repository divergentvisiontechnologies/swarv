<template>
  <div>
    <h1>All Recordings</h1>
    <center>
        <ul v-bind:key="audiorecording.id" v-for="audiorecording in audiorecordings">
      <SingleRecording v-bind:audiorecording="audiorecording"/>
    </ul>
    <!-- <div v-bind:key="audiorecording.id" v-for="audiorecording in audiorecordings">
        {{audiorecording.name}}
    </div> -->
    </center>
    
  </div>
</template>

<script>
import SingleRecording from "./SingleRecording.vue";
export default {
  name: "AllRecordings",
  components: {
    SingleRecording,
  },
  props: [
      "audiorecordings"
  ]
};
</script>

<style scoped>
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  width: 75vw;
  /* align-items: center; */
}
</style>
