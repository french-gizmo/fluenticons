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
<path d="m11.557 13.646-.083.071-6.927 6.8a3.234 3.234 0 0 0 1.703.481h4.914l.356-1.423c.162-.648.497-1.24.97-1.712l2.11-2.11-2.075-2.036-.094-.078a.75.75 0 0 0-.873.007Zm4.946-5.394a.752.752 0 1 0-1.504 0 .752.752 0 0 0 1.504 0Zm-.843 6.441-2.085-2.046-.128-.117a2.25 2.25 0 0 0-2.888-.006l-.136.123-6.938 6.81A3.234 3.234 0 0 1 3 17.75v-11.5A3.25 3.25 0 0 1 6.25 3h11.499a3.25 3.25 0 0 1 3.25 3.25v4.761a3.279 3.279 0 0 0-2.608.95l-2.731 2.732ZM13.5 8.252a2.252 2.252 0 1 0 4.503 0 2.252 2.252 0 0 0-4.504 0Zm5.598 4.417-5.901 5.901a2.685 2.685 0 0 0-.707 1.248l-.457 1.83c-.2.797.522 1.518 1.318 1.319l1.83-.458a2.685 2.685 0 0 0 1.248-.706L22.33 15.9a2.286 2.286 0 0 0-3.233-3.232Z" :fill="fill" :fill-opacity="opacity" /></svg>
</template>

<script>
import icon from "../../../mixins/icon.js"

export default {
    name: 'FluentIconFilledImageEdit',
    mixins: [icon]
};
</script>