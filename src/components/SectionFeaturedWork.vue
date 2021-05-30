<template>
  <BaseSection title="Featured Work">
    <iframe class="embedded" width="560" height="315" src="https://www.youtube.com/embed/OuAM-EueCBM"
        title="YouTube video player" frameborder="0"
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
        allowfullscreen></iframe>
    <iframe width="560" height="315" src="https://www.youtube.com/embed/yDQJPHuUc6Q" title="YouTube video player"
        frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
        allowfullscreen></iframe>
  </BaseSection>
</template>

<script>
import BaseSection from "@/components/BaseSection";

export default {
  name: "FeaturedWork",
  components: {BaseSection}
}
</script>

<style scoped>
.embedded {
  width: 100%;
}
</style>
