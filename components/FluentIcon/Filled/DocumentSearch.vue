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
<path d="M13 8V2H7a2 2 0 0 0-2 2v5.303a6 6 0 0 1 8.207 8.18l3.53 3.53c.278.277.443.626.495.987H19a2 2 0 0 0 2-2V10h-6a2 2 0 0 1-2-2Z" :fill="fill" :fill-opacity="opacity" />

<path d="M14.97 22.78a.75.75 0 1 0 1.06-1.06l-4.112-4.113A4.978 4.978 0 0 0 13 14.5a4.984 4.984 0 0 0-1.43-3.5A4.985 4.985 0 0 0 8 9.5a4.978 4.978 0 0 0-3 1 5 5 0 0 0 5.82 8.13l4.15 4.15ZM8 11a3.5 3.5 0 1 1 0 7 3.5 3.5 0 0 1 0-7ZM14.5 8V2.5l6 6H15a.5.5 0 0 1-.5-.5Z" :fill="fill" :fill-opacity="opacity" /></svg>
</template>

<script>
import icon from "../../../mixins/icon.js"

export default {
    name: 'FluentIconFilledDocumentSearch',
    mixins: [icon]
};
</script>