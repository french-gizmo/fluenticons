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
<path d="M2 8.5a6.503 6.503 0 0 0 4.943 6.312 7.993 7.993 0 0 1 1.716-4.806 1.992 1.992 0 0 0-1.68.694.75.75 0 0 1-1.14-.975 3.5 3.5 0 0 1 4.023-.95 7.995 7.995 0 0 1 4.95-1.832A6.5 6.5 0 0 0 2 8.5Zm5.5-2a1 1 0 1 1-2 0 1 1 0 0 1 2 0Zm4 0a1 1 0 1 1-2 0 1 1 0 0 1 2 0ZM22 15a7 7 0 1 1-14 0 7 7 0 0 1 14 0Zm-8.5-1.5a1 1 0 1 0-2 0 1 1 0 0 0 2 0Zm4.471 3.218a.625.625 0 0 0-.88.07 2.75 2.75 0 0 1-4.178.003.625.625 0 1 0-.948.814 3.998 3.998 0 0 0 6.075-.006.625.625 0 0 0-.069-.88ZM17.5 14.5a1 1 0 1 0 0-2 1 1 0 0 0 0 2Z" :fill="fill" :fill-opacity="opacity" /></svg>
</template>

<script>
import icon from "../../../mixins/icon.js"

export default {
    name: 'FluentIconFilledEmojiMultiple',
    mixins: [icon]
};
</script>