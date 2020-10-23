<template>
  <div class="app">
    <drum-button char="A" sound="clap" />
    <drum-button char="S" sound="hihat" />
    <drum-button char="D" sound="kick" />
    <drum-button char="F" sound="openhat" />
    <drum-button char="G" sound="boom" />
    <drum-button char="H" sound="ride" />
    <drum-button char="J" sound="snare" />
    <drum-button char="K" sound="tom" />
    <drum-button char="L" sound="tink" />
  </div>
</template>

<script>
import DrumButton from './components/DrumButton.vue'

export default {
  name: 'App',
  components: {
    DrumButton
  }
}
</script>

<style>
  .app {
    display: flex;
  }
</style>
