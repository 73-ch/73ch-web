<template>
  <BaseSection title="About">
    <div class="imgs about-content">
      <img src="@/assets/nami-logo.png" alt="">
      <img src="@/assets/nami-photo1.jpg" alt="photo of Tamika kosaku">
    </div>
    <div class="about-content">
      <p>Kosaku Namikawa / 浪川 洪作</p>
      <p>2000年生まれ、筑波大学情報学群所属</p>
      <p>システムから表現、マネージャーからエンジニア、クリエイターまで、プログラミングをバックボーンに分野・職域にとらわれ図に、デジタル技術を用いた制作活動・表現と向き合う。システムや技術の特性を活かした表現、また様々な技術を組み合わせた表現に関心がある。 </p>
      <p>15歳でプログラミングに出会い、Webのフルスタックエンジニアとしてサービス開発などを始める。16歳にはWebGLを通してリアルタイム3DCGに出会い、そこからopenFrameworksやGLSL, MaxMSPなどによる作品制作を開始。2018年より本格的にシステム開発やVJ、アーティストの作品制作補助、ワークショップのTAなど多角的に活動を開始。また、同年5月より観客のスマートフォンを用いたライブ演出システムの開発を始め、2018年度未踏ジュニアスーパークリエイター認定、平成30年度総務省異能vation破壊的な挑戦部門採択。現在は筑波大学に所属し、ものづくり集団TPartyのメンバーとしても活動を行う。</p>
    </div>
    <div class="about-content">
      <p><a href="https://www.instagram.com/73_ch/">Instagram</a></p>
      <p><a href="https://twitter.com/73_ch">Twitter</a></p>
      <p><a href="https://github.com/73-ch">GitHub</a></p>
      <p><a href="https://www.youtube.com/channel/UCMKhFmeN7xVWEa2AHSawa5w">YouTube</a></p>
    </div>
  </BaseSection>
</template>

<script>
import BaseSection from "@/components/BaseSection";

export default {
  name: "SectionAbout",
  components: {BaseSection}
}
</script>

<style scoped>
.imgs {
  width: 100%;
  display: flex;
  align-items: center;
  align-self: center;
  justify-content: space-around;
  flex-wrap: wrap;
}

.imgs img {
  min-height: 160px;
  height: 20vh;
}

p {
  margin: 10px 0;
}

.about-content {
  margin-bottom: 50px;
}
</style>
