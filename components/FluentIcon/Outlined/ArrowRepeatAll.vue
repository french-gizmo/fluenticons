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
<path d="m14.61 2.47-.077-.067a.748.748 0 0 0-.983.067l-.068.078a.755.755 0 0 0 .068.987l1.971 1.977H8.5l-.233.004C4.785 5.639 2 8.51 2 12.036c0 1.69.64 3.23 1.692 4.39l.072.069a.751.751 0 0 0 1.08-1.033l-.2-.231A5.009 5.009 0 0 1 3.5 12.035c0-2.771 2.239-5.018 5-5.018h6.881l-1.832 1.84-.067.078a.755.755 0 0 0 .068.987.748.748 0 0 0 1.06 0l3.182-3.193.067-.078a.755.755 0 0 0-.067-.987L14.61 2.47Zm5.62 5.101a.751.751 0 0 0-1.05 1.066 5.01 5.01 0 0 1 1.32 3.398c0 2.772-2.239 5.019-5 5.019H8.558l1.905-1.911.074-.086a.755.755 0 0 0-.007-.902l-.067-.077-.084-.073a.748.748 0 0 0-.9.006l-.076.067-3.182 3.194-.073.085a.755.755 0 0 0 .006.902l.067.077 3.182 3.194.084.072c.293.22.71.195.976-.073a.755.755 0 0 0 .068-.987l-.068-.077-1.899-1.906H15.5l.233-.004C19.215 18.432 22 15.56 22 12.035a6.513 6.513 0 0 0-1.697-4.395l-.073-.069Z" :fill="fill" :fill-opacity="opacity" /></svg>
</template>

<script>
import icon from "../../../mixins/icon.js"

export default {
    name: 'FluentIconOutlinedArrowRepeatAll',
    mixins: [icon]
};
</script>