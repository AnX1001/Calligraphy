<template>
  <div class="wrapper">
    <button>{{ btnText }}</button>
  </div>
</template>

<script>
export default {
  name: "ctaBtn",
  props: {
    btnText: {
      type: String,
    },
  },
};
</script>

<style lang="scss" scoped>
.wrapper {
  width: fit-content;
  button {
    width: fit-content;
    height: 35px;
    padding: 0 15px;
    background: black;
    color: white;
    border-radius: 3px;

    &:hover {
      cursor: pointer;
    }
  }
}
</style>
