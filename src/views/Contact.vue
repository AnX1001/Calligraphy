<template>
  <div class="home">
    <articleBlock
      :imgSrc="require('../assets/' + some)"
      :paragraph="paragraph"
      :heading="heading"
    >
    </articleBlock>
  </div>
</template>

<script>
// @ is an alias to /src
import articleBlock from "@/components/articleBlock.vue";

export default {
  name: "Home",
  components: {
    articleBlock,
  },
  data() {
    return {
      some: "some.jpg",
      heading: "Kontakt oss",
      paragraph: "Vi er på SoMe!",
    };
  },
};
</script>

<style lang="scss" scoped></style>
