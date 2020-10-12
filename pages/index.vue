<template>
  <div>
    <div id="typewriter">Hello my name is Kha-Yu Aimee Cheam</div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({})
</script>

<style>
#typewriter {
  font-size: 4vw;
  overflow: hidden;
  border-right: .1em solid orange;
  white-space: nowrap;
  margin: 0 auto;
  letter-spacing: .1em;
  animation:
    typing 4s steps(45,end),
    blink-caret .75s step-end 0s 10 forwards;
}

/* Type writer effect */
@keyframes typing {
  from {width: 0}
  to {width: 100%}
}

@keyframes blink-caret {
  from, to {border-color: transparent}
  50% {border-color: #ff9a8d;}
}
</style>
