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
<path d="M6 3.5h1v6.238c0 .375-.094.744-.273 1.074l-3.584 6.603A1.75 1.75 0 0 0 4.68 20h6.734l.106-.423c.096-.383.252-.746.461-1.077H4.681a.25.25 0 0 1-.22-.37l1.97-3.63h7.137l.805 1.482 1.106-1.106-2.206-4.064A2.25 2.25 0 0 1 13 9.738V3.5h1A.75.75 0 0 0 14 2H6a.75.75 0 0 0 0 1.5Zm2.5 6.238V3.5h3v6.238c0 .625.156 1.24.454 1.79l.8 1.472H7.246l.8-1.473A3.75 3.75 0 0 0 8.5 9.738Zm10.6 2.931-5.903 5.903a2.686 2.686 0 0 0-.706 1.247l-.458 1.831a1.087 1.087 0 0 0 1.319 1.318l1.83-.457a2.685 2.685 0 0 0 1.248-.707l5.902-5.902A2.286 2.286 0 0 0 19.1 12.67Z" :fill="fill" :fill-opacity="opacity" /></svg>
</template>

<script>
import icon from "../../../mixins/icon.js"

export default {
    name: 'FluentIconOutlinedBeakerEdit',
    mixins: [icon]
};
</script>