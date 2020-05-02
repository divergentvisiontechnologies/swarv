<template>
  <li>
    <div class="singleRecordingCard">
      <div id="detail-container">
        <h2>{{ audiorecording.name }}</h2>
        <!-- <h2>Title</h2> -->
        <p>
          {{ audiorecording.preface }}
          <!-- This is preface text -->
        </p>
      </div>

      <button id="btn_play" v-on:click="playAudio">Play</button>
    </div>
  </li>
</template>

<script>
export default {
  name: "SingleRecording",
  methods: {
    playAudio() {
      console.log("playing audio");
      alert("Playing: "+ this.audiorecording.name + " by " + this.audiorecording.artists)
    },
  },
  props: ["audiorecording"]
};
</script>

<style scoped>
#btn_play {
  background: #666;
  color: #ffffff;
  /* padding: 30.2px; */
  width: 25%;
  border: 0px;
}
#btn_play:hover {
  background: rgb(13, 194, 74);
}

h2 {
  color: rgb(37, 145, 233);
}
.singleRecordingCard {
  background: #000;
  color: #fff;
  overflow: hidden;
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: flex-start;
  border: 1px solid #999;
}
#detail-container {
  width: 75%;

  background-color: #000;
}
</style>
