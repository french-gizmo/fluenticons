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
<path d="M3.28 2.22a.75.75 0 1 0-1.06 1.06l1.045 1.046A2.5 2.5 0 0 0 2 6.5v9A2.5 2.5 0 0 0 4.5 18H9v-1.5H4.5a1 1 0 0 1-1-1v-9a1 1 0 0 1 .941-.998L10 11.06V21.25a.75.75 0 0 0 1.368.425l2.467-3.588 4.042.85 2.842 2.843a.75.75 0 0 0 1.061-1.06L3.28 2.22Zm8.22 10.34 4.435 4.436-2.28-.48a.75.75 0 0 0-.773.31l-1.382 2.01V12.56ZM20.5 15.5a1 1 0 0 1-.832.986l1.143 1.143A2.499 2.499 0 0 0 22 15.5v-9A2.5 2.5 0 0 0 19.5 4H7.182l1.5 1.5H19.5a1 1 0 0 1 1 1v9Z" :fill="fill" :fill-opacity="opacity" /></svg>
</template>

<script>
import icon from "../../../mixins/icon.js"

export default {
    name: 'FluentIconOutlinedCursorHoverOff',
    mixins: [icon]
};
</script>