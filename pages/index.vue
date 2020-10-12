<template>
  <div>
    <div id="typewriter">Hello my name is Kha-Yu Aimee Cheam</div>
    
    <div id="appear">
        <p>Senior @ PSU | Blue Band Trumpet | Hopeful Developer</p>
        <p>I like to code cools things, and learn many stuffs</p>
    </div>

  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
})
</script>

<style>
/* Type writer effect */
@keyframes typing {
  from {width: 0}
  to {width: 100%}
}

@keyframes blink-caret {
  from, to {border-color: transparent}
  50% {border-color: #ff9a8d;}
}

@keyframes timedAppearance {
  from { opacity: 0}
  to { opacity: 1}
}

#typewriter {
  font-size: 4vw;
  overflow: hidden;
  border-right: .1em solid orange;
  white-space: nowrap;
  margin: 0 auto;
  letter-spacing: .1em;
  animation:
    typing 3s steps(45,end),
    blink-caret .75s step-end 0s 10 forwards;
}

#appear p {
  animation-name: timedAppearance;
  animation-duration: 1s;
  animation-delay: 3s;
  animation-fill-mode: backwards;
}
</style>
