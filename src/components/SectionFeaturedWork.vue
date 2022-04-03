<template>
  <BaseSection title="Featured Works">
    <div class="embed-container">
      <element-featured-work title="Kosaku Namikawa / scrolling (2022)" url="https://scrolling.73ch.work/"
          image="thumbnails/thumbnail_scrolling.png"/>
      <element-featured-work title="Kosaku Namikawa & Yuta Okuyama / trajectory (2022)"
          url="https://confusion-sense-3df.notion.site/trajectory-6e2c0a04ab4d4e68b9b1276468053814  " image="thumbnails/thumbnail_trajectory.png"/>
      <element-featured-work title="Beyond Internet (2022)" url="https://confusion-sense-3df.notion.site/2021-Beyond-Internet-42c02cb24de6490396bdadc9d628a1d7"
          image="thumbnails/thumbnail_digicon.png"/>
      <element-featured-work title="TParty / シブキ (2021)" url="https://www.youtube.com/watch?v=tRubYTfBBGc"
          image="thumbnails/thumbnail_shibuki.png"/>
      <element-featured-work title="Kosaku Namikawa / presence (2021)" url="https://confusion-sense-3df.notion.site/ENDLESS-IMAGINARY-bef67a2477274bc687c0e98f069b2cfd"
          image="thumbnails/thumbnail_endless.png"/>
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
