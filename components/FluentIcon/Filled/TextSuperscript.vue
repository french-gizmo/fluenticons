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
<path d="M18.736 3.75c-.387 0-.736.365-.736.773a1 1 0 1 1-2 0c0-1.365 1.102-2.773 2.736-2.773.93 0 1.843.435 2.36 1.23.548.842.546 1.918-.052 2.936-.306.522-.722.908-1.105 1.21-.193.152-.39.292-.568.419l-.078.055c-.153.108-.292.206-.426.307a4.4 4.4 0 0 0-.41.343h1.994a1 1 0 0 1 0 2H17a1 1 0 0 1-1-1c0-1.517.902-2.367 1.664-2.941.161-.121.328-.238.48-.346l.073-.051c.177-.126.335-.24.482-.355.295-.233.494-.438.621-.654.27-.46.177-.714.1-.832-.108-.165-.352-.321-.684-.321Z" :fill="fill" :fill-opacity="opacity" />

<path d="m11.317 12 4.4-5.133c.133-.197.277-.375.425-.537a2 2 0 0 1-1.14-1.703L10 10.463 4.76 4.35a1 1 0 1 0-1.52 1.302L8.684 12l-5.442 6.35a1 1 0 0 0 1.518 1.3L10 13.538l5.24 6.114a1 1 0 0 0 1.52-1.302L11.316 12Z" :fill="fill" :fill-opacity="opacity" /></svg>
</template>

<script>
import icon from "../../../mixins/icon.js"

export default {
    name: 'FluentIconFilledTextSuperscript',
    mixins: [icon]
};
</script>