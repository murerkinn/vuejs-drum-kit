<template>
  <div>
    <div class="button" @click="makeSound()">
      <kbd>{{char}}</kbd>
    </div>

    <audio :id="sound" :src="`/audio/${sound}.wav`"/>
  </div>
</template>

<script>
export default {
  name: 'DrumButton',
  props: {
    char: String,
    sound: String
  },
  methods: {
    makeSound() {
      const aud = document.getElementById(this.sound);
      if(!aud) return;
      aud.play();
    }
  }
}
</script>

<style scoped>
  .button {
    width: 50px;
    height: 50px;
    background-color: red;
    border-radius: 7px;
    margin: 0 10px;
    text-align: center;
    padding: 10px;
    cursor: pointer;
  }
</style>
