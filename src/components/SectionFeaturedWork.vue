<template>
  <BaseSection title="Featured Work">
    <div class="embed-container">
      <iframe width="400" height="225" src="https://www.youtube.com/embed/tRubYTfBBGc" title="YouTube video player"
          frameborder="0"
          allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
          allowfullscreen></iframe>
      <iframe class="embedded" width="400" height="225" src="https://www.youtube.com/embed/OuAM-EueCBM"
          title="YouTube video player" frameborder="0"
          allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
          allowfullscreen></iframe>
      <iframe width="400" height="225" src="https://www.youtube.com/embed/yDQJPHuUc6Q" title="YouTube video player"
          frameborder="0"
          allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
          allowfullscreen></iframe>
    </div>
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
.embed-container {
  display: flex;
  flex-wrap: wrap;
}

.embed-container iframe {
  margin: 20px;
}
</style>
