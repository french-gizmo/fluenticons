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
<path d="M12 22c5.523 0 10-4.477 10-10S17.523 2 12 2 2 6.477 2 12s4.477 10 10 10Zm3.88-15.333a.625.625 0 0 1 .961.761l-.13.25a354.691 354.691 0 0 1-1.415 2.713 154.8 154.8 0 0 1-1.156 2.157c-.171.31-.326.586-.452.803a4.964 4.964 0 0 1-.32.5 1.875 1.875 0 0 1-2.94-2.327c.086-.109.244-.265.413-.425.182-.173.414-.387.678-.625a154.39 154.39 0 0 1 1.832-1.62 375.175 375.175 0 0 1 2.314-2.003l.214-.184Zm-7.946 10.46a.75.75 0 0 1-1.06 0 7.25 7.25 0 0 1 6.798-12.182.75.75 0 1 1-.344 1.46 5.75 5.75 0 0 0-5.393 9.661.75.75 0 0 1 0 1.06Zm9.954-7.985a.75.75 0 0 1 .955.46 7.25 7.25 0 0 1-1.716 7.524.75.75 0 1 1-1.061-1.06 5.75 5.75 0 0 0 1.362-5.969.75.75 0 0 1 .46-.955Z" :fill="fill" :fill-opacity="opacity" /></svg>
</template>

<script>
import icon from "../../../mixins/icon.js"

export default {
    name: 'FluentIconFilledGauge',
    mixins: [icon]
};
</script>