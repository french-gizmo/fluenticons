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
<path d="M3 18a1 1 0 1 0 2 0V6a1 1 0 0 0-2 0v12ZM19 18a1 1 0 1 0 2 0V6a1 1 0 1 0-2 0v12ZM13.786 13.8l-.085.097-.006.008a1 1 0 0 0 1.511 1.302l2.35-2.348c.274-.179.444-.504.444-.86s-.17-.681-.444-.86L15.2 8.785l-.098-.085-.008-.005a1 1 0 0 0-1.302.096l-.006.007-.085.098-.006.007a1 1 0 0 0 .097 1.302l.794.795h-3.19l-.022.002h-1.96l.801-.802.093-.11.006-.008a1 1 0 0 0-.01-1.177l-.005-.008-.091-.105-.117-.1-.008-.005a1 1 0 0 0-1.177.01l-.008.005-.098.084-2.36 2.359-.065.045-.007.006A1.035 1.035 0 0 0 6 12c0 .356.17.681.443.86L8.8 15.215l.098.085.008.005a1 1 0 0 0 1.399-1.399l-.006-.007-.085-.098-.8-.8h3.19l.022-.001h1.96l-.8.8Z" :fill="fill" :fill-opacity="opacity" /></svg>
</template>

<script>
import icon from "../../../mixins/icon.js"

export default {
    name: 'FluentIconFilledAutoFitWidth',
    mixins: [icon]
};
</script>