<template>
  <div class="home">
    <articleBlock
      :imgSrc="require('../assets/' + view)"
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
      view: "view.jpg",
      heading: "Historie",
      paragraph:
        "Kinesiske skrifttegn er et sett på flere tusen fonetisk-piktografiske tegn som brukes for å skrive kinesisk, japansk, koreansk, og også eldre former for vietnamesisk. Tegnsettet er i Taiwan, Korea og Japan kjent som henholdsvis hancha, hanja, og kanji. Hvert enkelt tegn representerer én stavelse. 30% av tegnene i daglig bruk er enstavelsesord.",
    };
  },
};
</script>

<style lang="scss" scoped></style>
