<template>
  <div class="copyright-copyright"
    ><div class="copyright-max-width max-content-container"
      ><span class="copyright-text"
        ><span class="copyright-text1"
          >© All rights reserved <span v-html="raw8sdo"></span></span
        ><a
          href="https://www.teleporthq.io"
          target="_blank"
          rel="noreferrer noopener"
          ><span class="copyright-text2">@TeleportHQ.</span></a
        ><span class="copyright-text3">
          Powered by <span v-html="rawvgsw"></span></span
        ><a
          href="https://www.vercel.com"
          target="_blank"
          rel="noreferrer noopener"
          ><span class="copyright-text4">Vercel</span></a
        ><span class="copyright-text5"
          >. Image source: <span v-html="rawnbyf"></span></span
        ><a
          href="https://www.unsplash.com"
          target="_blank"
          rel="noreferrer noopener"
          ><span class="copyright-text6">Unsplash</span></a
        ><span class="copyright-text7">.</span></span
      ></div
    ></div
  >
</template>

<script>
export default {
  name: 'Copyright',
  props: {},
  data() {
    return {
      raw8sdo: ' ',
      rawvgsw: ' ',
      rawnbyf: ' ',
    }
  },
}
</script>

<style scoped>
.copyright-copyright {
  flex: 0 0 auto;
  width: 100%;
  display: flex;
  align-items: center;
  padding-top: var(--dl-space-space-twounits);
  flex-direction: column;
  padding-bottom: var(--dl-space-space-twounits);
}
.copyright-max-width {
  align-items: stretch;
}
.copyright-text {
  color: var(--dl-color-grays-gray100);
  font-size: 14px;
  font-style: normal;
  font-weight: 300;
  line-height: 1.5;
}
.copyright-text1 {
  font-style: normal;
  font-weight: 300;
}
.copyright-text2 {
  font-style: normal;
  font-weight: 300;
  text-decoration: underline;
}
.copyright-text3 {
  font-style: normal;
  font-weight: 300;
}
.copyright-text4 {
  font-style: normal;
  font-weight: 300;
  text-decoration: underline;
}
.copyright-text5 {
  font-style: normal;
  font-weight: 300;
}
.copyright-text6 {
  font-style: normal;
  font-weight: 300;
  text-decoration: underline;
}
.copyright-text7 {
  font-style: normal;
  font-weight: 300;
}
@media(max-width: 991px) {
  .copyright-max-width {
    flex-direction: column;
  }
}
</style>
