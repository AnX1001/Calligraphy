<template>
  <div class="wrapper">
    <div class="inner-wrapper">
      <figure>
        <img :src="imgSrc" :alt="imgDesc" />
      </figure>
      <div class="links">
        <slot></slot>
      </div>
    </div>
    <hr />
  </div>
</template>

<script>
export default {
  name: "navBar",
  props: {
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
  width: 100%;
  height: 45px;

  .inner-wrapper {
    display: flex;

    .links {
      width: fit-content;
      display: flex;
      align-items: center;
    }
  }

  figure {
    width: 75px;
    display: flex;

    height: 45px;
    margin: 0 auto 0 0;

    img {
      width: 100%;
      height: 100%;
    }
  }

  hr {
    width: 100%;
    border: 0.1px solid black;
    background: lightgrey;
  }
}
</style>
