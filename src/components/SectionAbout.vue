<template>
  <BaseSection title="About">
    <div class="imgs about-content">
      <img src="@/assets/nami-logo.png" alt="">
      <img src="@/assets/nami-photo1.jpg" alt="photo of Tamika kosaku">
    </div>
    <div class="about-content">
      <p>Kosaku Namikawa / 浪川 洪作</p>
      <p>2000年生まれ、7ild3主宰、筑波大学大学院在籍</p>
      <p>私はメディアアーティストとして、技術や手法に依存しない表現の可能性を探究しています。表層的なアウトプットに留まらず、作品の根底にある「仕組み」や「構造」こそが表現の本質を形づくると考え、常にそれらの再解釈と再構築を試みています。特に、メディアにおける低レイヤー、すなわちプロトコルや信号、空間と物理の接続面など、普段意識されにくい階層に立ち戻ることによって、新たな表現方法を開拓することに魅力を感じています。</p>

      <p>私の制作は、メディア領域や職域を横断的（水平的）に移動しながら、それぞれに内在するレイヤー構造を縦断的（垂直的）に掘り下げるプロセスによって進められます。この自由な移動は、マクロな仕組みからミクロな技術仕様までを往還する視点をもたらし、作品に複層的な意味と構造を与えます。エンジニアリングに裏打ちされたこの思考法は、インスタレーション作品の設計や空間とのインターフェースの構築にも反映され、設置（インストール）そのものが作品の意味を生む装置となります。空間への配置、観客との関係性、場との相互作用は、作品を成立させるための構造であり、技術的実装と芸術的意図が交差するポイントです。インストールは物理的な設置作業であると同時に、意味と構造の関係性、そして作品そのものを確立するプロセスでもあります。</p>
      <p>私は、エンジニアリングの知見を活かしながら、メディアの内部構造を読み解き、横断的かつ多層的に再構築することで、表現の新たな表現を生み出すことを目指しています。技術は単なる手段ではなく、問いの出発点であり、概念の操作対象でもある。そうした視点から、メディアアートの実践を通じて、技術・空間・鑑賞者・概念の相互接続を再設計していきます。</p>
      <br>
      <p>Kosaku Namikawa / 73ch</p>
      <p>Born in 2000, founder of 7ild3, currently enrolled in the Graduate School of University of Tsukuba.</p>
      <p>As a media artist, I explore the possibilities of expression that do not depend on technology or methods. I believe that the essence of expression is shaped not only by superficial outputs but also by the "mechanisms" and "structures" underlying the works, and I constantly attempt to reinterpret and reconstruct them. In particular, I am fascinated by the idea of returning to low layers in media, such as protocols, signals, and the connections between space and physics, which are often overlooked, to develop new methods of expression.</p>
      <p>My work progresses through a process of traversing across media domains and professions, delving vertically into the inherent layer structures of each. This free movement provides a perspective that oscillates between macro mechanisms and micro technical specifications, giving the works a multi-layered meaning and structure. This engineering-backed way of thinking is reflected in the design of installation works and the construction of interfaces with space, where the installation itself becomes a device that generates the meaning of the work. The arrangement in space, the relationship with the audience, and the interaction with the place are structures that establish the work, intersecting technical implementation and artistic intent. Installation is not only a physical setup task but also a process that establishes the relationship between meaning and structure, as well as the work itself.</p>
      <p>I aim to create new expressions by interpreting the internal structures of media, reconstructing them in a horizontal and multi-layered manner, and utilizing my engineering knowledge. Technology is not just a means but also a starting point for questioning and an object of conceptual manipulation. Through the practice of media art, I will redesign the interconnections between technology, space, viewers, and concepts.</p>
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
