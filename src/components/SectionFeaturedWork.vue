<template>
  <BaseSection title="Featured Works">
    <div class="embed-container">
      <element-featured-work title="Kosaku Namikawa / scrolling (2022)" url="https://scrolling.73ch.work/"
          image="thumbnails/thumbnail_scrolling.png"/>
      <element-featured-work title="Kosaku Namikawa & Yuta Okuyama / trajectory (2022)"
          url="https://twitter.com/sozo_youth/status/1499322687831015425" image="thumbnails/thumbnail_trajectory.png"/>
      <element-featured-work title="Beyond Internet (2022)" url="https://digicon.mast.tsukuba.ac.jp/"
          image="thumbnails/thumbnail_digicon.png"/>
      <element-featured-work title="TParty / シブキ (2021)" url="https://www.youtube.com/watch?v=tRubYTfBBGc"
          image="thumbnails/thumbnail_shibuki.png"/>
      <element-featured-work title="Kosaku Namikawa & Rensho Takahashi / Juggling Movie (2021)"
          url="https://www.youtube.com/watch?v=yDQJPHuUc6Q" image="thumbnails/thumbnail_juggling.png"/>
      <element-featured-work title="TParty / invisible (2021)" url="https://www.youtube.com/watch?v=-ih5usyWJW4"
          image="thumbnails/thumbnail_invisible.png"/>
    </div>
  </BaseSection>
</template>

<script>
import BaseSection from "@/components/BaseSection";
import ElementFeaturedWork from "@/components/ElementFeaturedWork";

export default {
  name: "FeaturedWork",
  components: {
    BaseSection,
    ElementFeaturedWork
  }
}
</script>

<style scoped>
.embed-container {
  display: flex;
  flex-wrap: wrap;
}

.embed-container iframe {
  /*margin: 20px;*/
}
</style>
