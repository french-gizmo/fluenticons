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
<path d="M17.5 3.992a2.5 2.5 0 0 1 2.5 2.5v4a1 1 0 1 1-2 0v-4a.5.5 0 0 0-.5-.5h-11a.5.5 0 0 0-.5.5v4a1 1 0 1 1-2 0v-4a2.5 2.5 0 0 1 2.5-2.5h11ZM18.2 13.036l-.098-.084-.008-.006a1 1 0 0 0-1.399 1.4l.006.007.085.098.8.799h-3.19l-.107.008-.01.002c-.464.072-.779.51-.779.99s.315.918.779.99l.01.002.108.008h3.19l-.802.802-.093.11-.006.008a1 1 0 0 0 .01 1.177l.005.007.091.106.117.099.008.006a1 1 0 0 0 1.177-.01l.008-.005.098-.085 2.36-2.358.065-.046.007-.005c.229-.186.368-.482.368-.805 0-.356-.17-.681-.443-.86L18.2 13.035ZM7.274 14.355l-.085.099-.8.799h3.18c.53 0 .906.48.906 1 0 .48-.315.918-.78.99l-.009.002-.108.008h-3.19l.795.794a1 1 0 0 1 .096 1.303l-.005.007-.085.098-.006.007a1 1 0 0 1-1.303.096l-.007-.005-.098-.085-2.357-2.354a1.023 1.023 0 0 1-.443-.86c0-.356.17-.682.443-.86l2.35-2.348a1 1 0 0 1 1.511 1.302l-.005.007Z" :fill="fill" :fill-opacity="opacity" /></svg>
</template>

<script>
import icon from "../../../mixins/icon.js"

export default {
    name: 'FluentIconFilledArrowAutofitWidth',
    mixins: [icon]
};
</script>