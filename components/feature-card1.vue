<template>
  <div class="feature-card1-card" v-bind:class="rootClassName"
    ><div class="feature-card1-container"><slot></slot></div
    ><h4 class="feature-card1-text Heading4">{{ heading }}</h4
    ><span class="feature-card1-text1 Content-Light">{{ text }}</span></div
  >
</template>

<script>
export default {
  name: 'FeatureCard1',
  props: {
    rootClassName: String,
    heading: {
      type: String,
      default: 'Search for ideas',
    },
    text: {
      type: String,
      default:
        'Amet minim mollit non deserunt ullamco est sit aliqua dolor do amet sint. Velit officia consequat duis enim velit mollit.',
    },
  },
}
</script>

<style scoped>
.feature-card1-card {
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
.feature-card1-container {
  flex: 0 0 auto;
  width: 200px;
  display: flex;
  align-items: center;
  margin-bottom: var(--dl-space-space-halfunit);
  flex-direction: column;
  justify-content: flex-start;
}
.feature-card1-text {
  text-align: center;
  margin-bottom: var(--dl-space-space-unit);
}
.feature-card1-text1 {
  color: var(--dl-color-grays-gray100);
  text-align: center;
  margin-bottom: var(--dl-space-space-unit);
}




@media(max-width: 767px) {
  .feature-card1-card {
    width: 50%;
  }
}
@media(max-width: 479px) {
  .feature-card1-card {
    width: 100%;
  }
}
</style>
