<template>
  <div class="video-container">
    <iframe :src="src" frameborder="0" allowfullscreen="true" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" />
  </div>
</template>

<script>
export default {
  props: {
    maxWidth: {
      type: String,
      required: false,
      default: null
    },
    videoId: {
      type: String,
      required: true
    }
  },
  computed: {
    src () {
      return `https://www.youtube.com/embed/${this.videoId}`
    }
  }
}
</script>

<style lang="scss" scoped>
.video-container {
  overflow: hidden;
  position: relative;
  width:100%;

  &:after {
    padding-top: 56.25%;
    display: block;
    content: '';
  }

  iframe {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
  }
}
</style>
