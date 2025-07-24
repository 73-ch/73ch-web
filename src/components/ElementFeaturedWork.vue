<template>
  <div class="container-featured-work">

    <a class="overlay-featured-work" :href="url" target="_blank">
      <h3 class="title-featured-work">{{ title }}</h3>
    </a>
    <img class="thumbnail-featured-work" :src="image" :alt="`thumbnail of ${this.title}`">

  </div>
</template>

<script>
export default {
  name: "ElementFeaturedWork",
  props: {
    title: {
      type: String,
      required: true
    },
    url: {
      type: String,
      default: ""
    },
    image: {
      type: String,
      required: true
    }
  },
  methods: {
    clickLink() {
      if (this.url.length === 0) return;

      window.open(this.url);
    }
  }
}
</script>

<style scoped>
.container-featured-work {
  position: relative;
  width: 400px;
  height: 225px;
}

.thumbnail-featured-work {
  width: 100%;
  height: 100%;
  display: block;
  object-fit: cover;
}

.container-featured-work:hover .overlay-featured-work {
  opacity: 1;
}

.overlay-featured-work {
  width: 100%;
  height: 100%;
  display: block;
  background-color: #444444;

  position: absolute;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  opacity: 0;
  transition: .5s ease;
}

.title-featured-work {
  color: white;
  position: absolute;
  top: 50%;
  left: 50%;
  -webkit-transform: translate(-50%, -50%);
  -ms-transform: translate(-50%, -50%);
  transform: translate(-50%, -50%);
  text-align: center;
  z-index: 10;
  /*transform: translate(50%, 50%);*/
}
</style>
