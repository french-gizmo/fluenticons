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
<path d="M12 2a3.75 3.75 0 0 0-3.736 3.424A7.999 7.999 0 0 0 4 12.5V14h16v-1.5a7.999 7.999 0 0 0-4.264-7.076A3.75 3.75 0 0 0 12 2Zm8 13.714H9.5v1.536a.75.75 0 0 1-1.5 0v-1.536H4v3.036A3.25 3.25 0 0 0 7.25 22h9.5A3.25 3.25 0 0 0 20 18.75v-3.036ZM12 4.5c-.698 0-1.374.09-2.02.257a2.25 2.25 0 0 1 4.04 0A8.013 8.013 0 0 0 12 4.5Zm-4 5.917A2.417 2.417 0 0 1 10.417 8h3.166A2.417 2.417 0 0 1 16 10.417C16 11.29 15.291 12 14.417 12H9.583A1.583 1.583 0 0 1 8 10.417Zm2.417-.917a.917.917 0 0 0-.917.917c0 .046.037.083.083.083h4.834a.083.083 0 0 0 .083-.083.917.917 0 0 0-.917-.917h-3.166Z" :fill="fill" :fill-opacity="opacity" /></svg>
</template>

<script>
import icon from "../../../mixins/icon.js"

export default {
    name: 'FluentIconFilledBackpack',
    mixins: [icon]
};
</script>