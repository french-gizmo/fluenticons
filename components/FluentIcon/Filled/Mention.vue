<template>
    <svg width="24" height="24" fill="none" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
<linearGradient v-if="fill === 'url(#g1)'" id="g1" :gradientTransform="`rotate(${angle})`">
      <stop class="main-stop" offset="0%" :stop-color="start" />
      <stop class="alt-stop" offset="100%" :stop-color="end" />
    </linearGradient>
    <radialGradient v-if="fill === 'url(#g2)'" id="g2" cx = "50%" cy = "50%" r = "50%">
      <stop :stop-color="start" offset = "0%"/>
      <stop :stop-color="end" offset = "100%"/>
    </radialGradient>
<path d="M12 2c5.43 0 9.848 4.327 9.996 9.72L22 12v1.525a4 4 0 0 1-7.415 2.06c-.8.833-1.882 1.348-3.085 1.348-2.515 0-4.5-2.25-4.5-4.966C7 9.25 8.985 7 11.5 7c.937 0 1.8.312 2.514.844a1 1 0 0 1 1.98.04L16 8v5.5a2 2 0 0 0 3.994.15l.006-.175V12a8 8 0 1 0-8 8c.921 0 1.82-.155 2.67-.456a1 1 0 1 1 .667 1.886A9.985 9.985 0 0 1 12 22C6.477 22 2 17.523 2 12S6.477 2 12 2Zm-.35 7.005L11.5 9C10.15 9 9 10.302 9 11.967c0 1.664 1.15 2.966 2.5 2.966 1.3 0 2.415-1.207 2.495-2.783l.005-.22c-.017-1.586-1.075-2.834-2.35-2.925L11.5 9l.15.005Z" :fill="fill" :fill-opacity="opacity" /></svg>
</template>

<script>
import icon from "../../../mixins/icon.js"

export default {
    name: 'FluentIconFilledMention',
    mixins: [icon]
};
</script>