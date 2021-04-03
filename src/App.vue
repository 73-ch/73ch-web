<template>
  <div id="app">
    <SectionTop/>
    <SectionAbout/>
    <SectionFeaturedWork/>
    <SectionWorks/>
    <SectionCopyright/>
  </div>
</template>

<script>
import '@/assets/ress.css'

import SectionTop from "@/components/SectionTop";
import SectionAbout from "@/components/SectionAbout";
import SectionFeaturedWork from "@/components/SectionFeaturedWork"
import SectionWorks from "@/components/SectionWorks";
import SectionCopyright from "@/components/SectionCopyright";

export default {
  name: 'App',
  components: {
    SectionTop,
    SectionAbout,
    SectionFeaturedWork,
    SectionWorks,
    SectionCopyright
  }
}
</script>

<style>
#app {
  max-width: 800px;
  margin: 0 5vw;

  font-family: Avenir, Helvetica, Arial, sans-serif;
  color: #222324;
}

a {
  color: #222324;
  text-decoration: none;
}

a:hover {
  opacity: 40%;
}

a:visited {
  color: #222324;
}

* {
  word-wrap: break-word;
  overflow-wrap : break-word;
}

</style>
