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
<path d="M3.5 5.25c0-.966.784-1.75 1.75-1.75h3a.75.75 0 0 0 0-1.5h-3A3.25 3.25 0 0 0 2 5.25v3a.75.75 0 0 0 1.5 0v-3Zm17 0a1.75 1.75 0 0 0-1.75-1.75h-3a.75.75 0 0 1 0-1.5h3A3.25 3.25 0 0 1 22 5.25v3a.75.75 0 0 1-1.5 0v-3ZM5.25 20.5a1.75 1.75 0 0 1-1.75-1.75v-3a.75.75 0 0 0-1.5 0v3A3.25 3.25 0 0 0 5.25 22h3a.75.75 0 0 0 0-1.5h-3Zm15.25-1.75a1.75 1.75 0 0 1-1.75 1.75h-3a.75.75 0 0 0 0 1.5h3A3.25 3.25 0 0 0 22 18.75v-3a.75.75 0 0 0-1.5 0v3ZM11.29 6.424c.264-.615 1.063-1.404 2.179-1.115.7.182 1.204.601 1.489 1.178.248.502.29 1.05.3 1.466.008.397-.056.828-.138 1.214h.194c1.558 0 2.822 1.433 2.332 2.991l-1.15 3.654c-.465 1.482-2.1 2.25-3.577 1.817l-4.512-1.323a2.391 2.391 0 0 1-1.557-1.387l-.438-1.089c-.439-1.09.04-2.286 1.055-2.845l1.542-.85a2.584 2.584 0 0 0 .293-.268c.239-.25.596-.7.962-1.428.178-.352.327-.63.459-.874v-.002c.213-.395.378-.7.566-1.139Z" :fill="fill" :fill-opacity="opacity" /></svg>
</template>

<script>
import icon from "../../../mixins/icon.js"

export default {
    name: 'FluentIconFilledScanThumbUp',
    mixins: [icon]
};
</script>