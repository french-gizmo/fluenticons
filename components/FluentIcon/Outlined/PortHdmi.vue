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
<path d="m21.414 11.414-2.828-2.828A2 2 0 0 0 17.172 8H6.828a2 2 0 0 0-1.414.586l-2.828 2.828A2 2 0 0 0 2 12.828V14a2 2 0 0 0 2 2h16a2 2 0 0 0 2-2v-1.172a2 2 0 0 0-.586-1.414ZM20.5 14a.5.5 0 0 1-.5.5H4a.5.5 0 0 1-.5-.5v-1.172a.496.496 0 0 1 .146-.353l2.829-2.828a.497.497 0 0 1 .353-.147h10.344a.497.497 0 0 1 .353.146l2.829 2.829a.495.495 0 0 1 .146.354V14Zm-4.25-2.75h-8.5a.75.75 0 1 0 0 1.5h8.5a.75.75 0 1 0 0-1.5Z" :fill="fill" :fill-opacity="opacity" /></svg>
</template>

<script>
import icon from "../../../mixins/icon.js"

export default {
    name: 'FluentIconOutlinedPortHdmi',
    mixins: [icon]
};
</script>