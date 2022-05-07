<template>
  <div class="wrapper">
    <figure>
      <img :src="imgSrc" :alt="imgDesc" />
      <figcaption>{{ figCaption }}</figcaption>
    </figure>
  </div>
</template>

<script>
export default {
  name: "lazyImage",
  props: {
    figCaption: {
      type: String,
    },
    imgSrc: {
      type: String,
    },
    imgDesc: {
      type: String,
    },
  },
};
</script>

<style lang="scss" scoped>
.wrapper {
  width: fit-content;

  figure {
    margin: 0;
    img {
      width: 100%;
      height: auto;
      max-height: 570px;
      border-radius: 3px;
      background-size: cover;
      background-repeat: no-repeat;
    }
  }
}
</style>
