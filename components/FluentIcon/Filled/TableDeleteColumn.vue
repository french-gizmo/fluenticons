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
<path d="M22 3.75V8h-5V6.25A3.25 3.25 0 0 1 20.25 3h1a.75.75 0 0 1 .75.75ZM22 9.5v5h-5v-5h5ZM21.25 21a.75.75 0 0 0 .75-.75V16h-5v1.75A3.25 3.25 0 0 0 20.25 21h1ZM2 20.25c0 .414.336.75.75.75h1A3.25 3.25 0 0 0 7 17.75V16H2v4.25ZM2 9.5v5h5v-5H2ZM2 3.75V8h5V6.25A3.25 3.25 0 0 0 3.75 3h-1a.75.75 0 0 0-.75.75ZM11.25 15.523v5.727a.75.75 0 0 0 1.5 0v-5.727a1.826 1.826 0 0 1-.076-.072L12 14.777l-.674.674-.076.072ZM11.25 8.727c.026.023.051.047.076.072l.674.674.674-.674c.025-.025.05-.049.076-.072V2.75a.75.75 0 0 0-1.5 0v5.977Z" :fill="fill" :fill-opacity="opacity" />

<path d="M9.47 14.53a.75.75 0 0 1 0-1.06L10.94 12l-1.47-1.47a.75.75 0 1 1 1.06-1.06L12 10.94l1.47-1.47a.75.75 0 1 1 1.06 1.06L13.06 12l1.47 1.47a.75.75 0 1 1-1.06 1.06L12 13.06l-1.47 1.47a.75.75 0 0 1-1.06 0Z" :fill="fill" :fill-opacity="opacity" /></svg>
</template>

<script>
import icon from "../../../mixins/icon.js"

export default {
    name: 'FluentIconFilledTableDeleteColumn',
    mixins: [icon]
};
</script>