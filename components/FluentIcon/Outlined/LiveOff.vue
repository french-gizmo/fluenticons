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
<path d="M3.28 2.22a.75.75 0 1 0-1.06 1.06L4.418 5.48c-3.386 3.929-3.216 9.865.51 13.592a.75.75 0 1 0 1.062-1.06 8.5 8.5 0 0 1-.508-11.468L7.26 8.321a6.001 6.001 0 0 0 .497 7.922.75.75 0 0 0 1.061-1.061 4.501 4.501 0 0 1-.486-5.79l2.219 2.22A1.503 1.503 0 0 0 12 13.5c.134 0 .264-.018.388-.05l8.331 8.33a.75.75 0 0 0 1.061-1.06L3.28 2.22ZM19.389 16.207l1.093 1.094c2.418-3.861 1.947-9.014-1.41-12.372a.75.75 0 0 0-1.062 1.06 8.504 8.504 0 0 1 1.378 10.218ZM16.347 13.165l1.178 1.178a6.002 6.002 0 0 0-1.282-6.586.75.75 0 1 0-1.061 1.061 4.498 4.498 0 0 1 1.165 4.348Z" :fill="fill" :fill-opacity="opacity" /></svg>
</template>

<script>
import icon from "../../../mixins/icon.js"

export default {
    name: 'FluentIconOutlinedLiveOff',
    mixins: [icon]
};
</script>