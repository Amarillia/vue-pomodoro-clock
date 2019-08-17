<template>
  <div id="app">
    <AppButton name="Break Decrement" id="break-decrement" />
    <AppButton name="Session Decrement" id="session-decrement" />
    <AppButton name="Break Increment" id="break-increment" />
    <AppButton name="Session Increment" id="session-increment" />
    <p name="Break Length" id="break-label"></p>
    <p name="Session Length" id="session-label"></p>
    <p name="Session" id="timer-label"></p>
    <p name="Time Left" id="time-left">
      <span id="timer-mins" class="timer">25:</span>
      <span id="timer-secs" class="timer">00</span>
    </p>
  </div>
</template>

<script>
import AppButton from "./components/AppButton.vue";

export default {
  name: "app",
  components: {
    AppButton
  }
};
</script>

<style>
/* Colours */
/* #A66D78
#BF9B6F
#BF8069
#D96B62 */

* {
  background-color: #590209;
  color: #fff;
}

#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.timer {
  font-size: 100px;
}
</style>
