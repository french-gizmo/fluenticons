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
<path d="M21.78 2.22a.75.75 0 0 1 0 1.06L18.56 6.5l3.22 3.22a.75.75 0 1 1-1.06 1.06L17.5 7.56l-3.22 3.22a.75.75 0 1 1-1.06-1.06l3.22-3.22-3.22-3.22a.75.75 0 0 1 1.06-1.06l3.22 3.22 3.22-3.22a.75.75 0 0 1 1.06 0ZM9.367 3.312l.86 2.028c.374.883.167 1.922-.514 2.568L7.819 9.706c.116 1.076.478 2.135 1.084 3.177a8.678 8.678 0 0 0 2.271 2.595l2.275-.76c.863-.287 1.802.044 2.33.821l1.233 1.81c.615.904.505 2.15-.258 2.916l-.818.821c-.814.817-1.977 1.114-3.052.778-2.539-.792-4.873-3.143-7.003-7.053-2.133-3.916-2.886-7.24-2.258-9.968.264-1.148 1.081-2.063 2.149-2.404l1.076-.344c1.01-.322 2.087.199 2.52 1.217Z" :fill="fill" :fill-opacity="opacity" /></svg>
</template>

<script>
import icon from "../../../mixins/icon.js"

export default {
    name: 'FluentIconFilledCallDismiss',
    mixins: [icon]
};
</script>