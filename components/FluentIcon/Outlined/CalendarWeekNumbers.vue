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
<path d="M17.75 3A3.25 3.25 0 0 1 21 6.25v11.5A3.25 3.25 0 0 1 17.75 21H6.25A3.25 3.25 0 0 1 3 17.75V6.25A3.25 3.25 0 0 1 6.25 3h11.5Zm0 1.5H6.25A1.75 1.75 0 0 0 4.5 6.25v11.5c0 .966.784 1.75 1.75 1.75h11.5a1.75 1.75 0 0 0 1.75-1.75V6.25a1.75 1.75 0 0 0-1.75-1.75ZM7.75 7a.75.75 0 0 1 .743.648l.007.102v1a.75.75 0 0 1-1.493.102L7 8.75v-1A.75.75 0 0 1 7.75 7Z" :fill="fill" :fill-opacity="opacity" />

<path d="M8.493 15.148A.75.75 0 0 0 7 15.25v1l.007.102A.75.75 0 0 0 8.5 16.25v-1l-.007-.102ZM8.5 11.321a.75.75 0 0 0-1.493.102L7 12.57l.007.102A.75.75 0 0 0 8.5 12.57l.007-1.148-.007-.102Z" :fill="fill" :fill-opacity="opacity" /></svg>
</template>

<script>
import icon from "../../../mixins/icon.js"

export default {
    name: 'FluentIconOutlinedCalendarWeekNumbers',
    mixins: [icon]
};
</script>