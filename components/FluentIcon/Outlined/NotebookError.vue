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
<path d="M6.5 12a5.5 5.5 0 1 1 0 11 5.5 5.5 0 0 1 0-11ZM16.749 2a2.25 2.25 0 0 1 2.25 2.25v15.5a2.25 2.25 0 0 1-2.25 2.25h-5.56c.427-.443.791-.948 1.078-1.499l4.482-.001a.75.75 0 0 0 .75-.75V4.25a.75.75 0 0 0-.75-.75H6.25a.75.75 0 0 0-.75.75v6.826a6.457 6.457 0 0 0-1.5.422V4.25A2.25 2.25 0 0 1 6.25 2h10.499ZM6.5 19.88a.625.625 0 1 0 0 1.249.625.625 0 0 0 0-1.249Zm0-5.877a.5.5 0 0 0-.492.41l-.008.09v3.998l.008.09a.5.5 0 0 0 .984 0L7 18.5v-3.998l-.008-.09a.5.5 0 0 0-.492-.41Zm14.25.999a.75.75 0 0 1 .743.648l.007.102v1.498a.75.75 0 0 1-.648.743L20.75 18H20v-2.998h.75Zm0-4a.75.75 0 0 1 .743.648l.007.102v1.498a.75.75 0 0 1-.648.743L20.75 14H20v-2.998h.75Zm0-4a.75.75 0 0 1 .743.648l.007.102V9.25a.75.75 0 0 1-.648.743L20.75 10H20V7.002h.75ZM15.249 5a.75.75 0 0 1 .75.75v2.498a.75.75 0 0 1-.75.75H7.75a.75.75 0 0 1-.75-.75V5.75A.75.75 0 0 1 7.75 5h7.499Zm-.75 1.5H8.5v.998h5.999V6.5Z" :fill="fill" :fill-opacity="opacity" /></svg>
</template>

<script>
import icon from "../../../mixins/icon.js"

export default {
    name: 'FluentIconOutlinedNotebookError',
    mixins: [icon]
};
</script>