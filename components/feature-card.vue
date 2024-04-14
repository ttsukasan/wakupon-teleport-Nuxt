<template>
  <div class="feature-card-card"
    ><img :alt="imageAlt" :src="imageSrc" class="feature-card-image" /><h4
      class="feature-card-text Heading4"
      >{{ heading }}</h4
    ><span class="feature-card-text1 Content-Light">{{ text }}</span></div
  >
</template>

<script>
export default {
  name: 'FeatureCard',
  props: {
    text1: {
      type: String,
      default: 'Get started >',
    },
    text: {
      type: String,
      default:
        'Amet minim mollit non deserunt ullamco est sit aliqua dolor do amet sint. Velit officia consequat duis enim velit mollit.',
    },
    heading: {
      type: String,
      default: 'Search for ideas',
    },
    imageAlt: {
      type: String,
      default: 'image',
    },
    imageSrc: {
      type: String,
      default: 'https://play.teleporthq.io/static/svg/default-img.svg',
    },
  },
}
</script>

<style scoped>
.feature-card-card {
  flex: 0 0 auto;
  width: 25%;
  display: flex;
  max-width: 285px;
  align-items: center;
  padding-top: var(--dl-space-space-oneandhalfunits);
  padding-left: var(--dl-space-space-unit);
  padding-right: var(--dl-space-space-unit);
  flex-direction: column;
  padding-bottom: var(--dl-space-space-oneandhalfunits);
}
.feature-card-image {
  width: 60px;
  height: 60px;
  object-fit: cover;
  margin-bottom: var(--dl-space-space-twounits);
}
.feature-card-text {
  text-align: center;
  margin-bottom: var(--dl-space-space-unit);
}
.feature-card-text1 {
  color: var(--dl-color-grays-gray100);
  text-align: center;
  margin-bottom: var(--dl-space-space-unit);
}
@media(max-width: 767px) {
  .feature-card-card {
    width: 50%;
  }
}
@media(max-width: 479px) {
  .feature-card-card {
    width: 100%;
  }
}
</style>
