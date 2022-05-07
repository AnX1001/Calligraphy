<template>
  <div class="wrapper">
    <article>
      <div class="text">
        <h1>{{ heading }}</h1>
        <p>{{ paragraph }}</p>
      </div>

      <lazyImage :imgSrc="imgSrc" class="image"></lazyImage>
    </article>
  </div>
</template>

<script>
import lazyImage from "./lazyImage.vue";
export default {
  components: { lazyImage },
  name: "articleBlock",
  props: {
    imgSrc: {
      type: String,
    },
    paragraph: {
      type: String,
    },
    heading: {
      type: String,
    },
  },
  data() {
    return {};
  },
};
</script>

<style lang="scss" scoped>
.wrapper {
  width: 100%;

  article {
    h1 {
      width: fit-content;
    }

    .image {
      width: 100%;
    }

    p {
      height: fit-content;
      width: fit-content;
    }
  }
}

@media (min-width: 768px) {
  .wrapper {
    width: 100%;
    margin-top: 30px;
    display: flex;
    justify-content: center;

    article {
      display: flex;
      flex-direction: row-reverse;

      .text {
        width: 365px;
        padding: 10px;
      }

      .image {
        width: 400px;
        height: auto;
        margin-right: 25px;
        margin-left: 25px;
      }
    }
  }
}
</style>
