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
<path d="M8 2H5a3 3 0 0 0-3 3v3h2.708A2.5 2.5 0 0 1 8 4.708V2ZM2 9.5V14a3 3 0 0 0 3 3h3v-6.44l-1.72 1.72a.75.75 0 0 1-1.06-1.06L6.94 9.5H2ZM9.5 17h1.519A6.5 6.5 0 0 1 22 12.81V9.5H10.56l1.72 1.72a.75.75 0 1 1-1.06 1.06L9.5 10.56V17ZM22 8h-9.208A2.5 2.5 0 0 0 9.5 4.708V2H19a3 3 0 0 1 3 3v3ZM10.5 8h-1V7a1 1 0 1 1 1 1ZM8 8H7a1 1 0 1 1 1-1.008V8Zm15 9.5a5.5 5.5 0 1 0-11 0 5.5 5.5 0 0 0 11 0Zm-5 .5.001 2.503a.5.5 0 1 1-1 0V18h-2.505a.5.5 0 0 1 0-1H17v-2.5a.5.5 0 1 1 1 0V17h2.497a.5.5 0 0 1 0 1H18Z" :fill="fill" :fill-opacity="opacity" /></svg>
</template>

<script>
import icon from "../../../mixins/icon.js"

export default {
    name: 'FluentIconFilledGiftCardAdd',
    mixins: [icon]
};
</script>