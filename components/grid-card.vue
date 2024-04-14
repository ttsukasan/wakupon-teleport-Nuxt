<template>
  <div class="grid-card-grid-card" v-bind:class="rootClassName"
    ><div class="grid-card-container"
      ><img :alt="imageAlt" :src="imageSrc" class="grid-card-image" /><div
        class="grid-card-container1"
        ><h2 class="grid-card-text">{{ heading }}</h2></div
      ></div
    ><button type="button" class="grid-card-button button-primary button"
      >{{ button }}</button
    ><span class="Content-Light">{{ text1 }}</span></div
  >
</template>

<script>
export default {
  name: 'GridCard',
  props: {
    heading: {
      type: String,
      default: 'Heading',
    },
    button: {
      type: String,
      default: 'インストール',
    },
    rootClassName: String,
    text1: {
      type: String,
      default:
        'Lorem ipsum dolor sit amet. Velit officia lorem ipsum dolor consequat duis enim velit mollit.​',
    },
    imageSrc: {
      type: String,
      default: 'https://play.teleporthq.io/static/svg/default-img.svg',
    },
    imageAlt: {
      type: String,
      default: 'image',
    },
  },
}
</script>

<style scoped>
.grid-card-grid-card {
  flex: 0 0 auto;
  width: 100%;
  display: flex;
  padding: 36px;
  align-items: flex-start;
  flex-direction: column;
  background-color: var(--dl-color-grays-white100);
}
.grid-card-container {
  flex: 0 0 auto;
  width: auto;
  height: 60px;
  display: flex;
  align-items: flex-start;
  margin-bottom: var(--dl-space-space-unit);
  justify-content: flex-start;
}
.grid-card-image {
  width: 60px;
  height: 60px;
  object-fit: cover;
  margin-bottom: var(--dl-space-space-oneandhalfunits);
}
.grid-card-container1 {
  flex: 0 0 auto;
  width: 200px;
  height: 100%;
  display: flex;
  align-items: flex-start;
  flex-direction: column;
  justify-content: center;
}
.grid-card-text {
  margin-left: var(--dl-space-space-unit);
}
.grid-card-button {
  margin-bottom: var(--dl-space-space-unit);
}
</style>
