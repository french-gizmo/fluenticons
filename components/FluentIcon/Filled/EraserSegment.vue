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
<path d="M12.651 2.638a2.25 2.25 0 0 1 3.19.023l4.91 5.008a2.25 2.25 0 0 1-.007 3.158L12.16 19.5h3.954a2.501 2.501 0 1 1 0 1.5H9.848a2.244 2.244 0 0 1-1.69-.642L3.06 15.35a2.25 2.25 0 0 1-.007-3.204l9.598-9.508ZM9.801 19.5a.747.747 0 0 0 .467-.22l1.468-1.483-6.099-6.1-1.529 1.515a.75.75 0 0 0 .003 1.068l5.099 5.008c.15.147.345.218.54.214V19.5h.05Z" :fill="fill" :fill-opacity="opacity" /></svg>
</template>

<script>
import icon from "../../../mixins/icon.js"

export default {
    name: 'FluentIconFilledEraserSegment',
    mixins: [icon]
};
</script>