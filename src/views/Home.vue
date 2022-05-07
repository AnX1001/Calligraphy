<template>
  <div class="home">
    <div class="wrapper">
      <articleBlock
        :imgSrc="require('../assets/' + calligraphy)"
        :paragraph="paragraph"
        :heading="heading"
      >
      </articleBlock>

      <ctaBtn :btnText="btnText" class="btn"></ctaBtn>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import articleBlock from "@/components/articleBlock.vue";
import ctaBtn from "@/components/ctaBtn.vue";

export default {
  name: "Home",
  components: {
    articleBlock,
    ctaBtn,
  },
  data() {
    return {
      calligraphy: "calligraphy.jpg",
      heading: "Kinesisk kalligrafi",
      paragraph:
        "Lyst til å prøve noe nytt? Hva med kinesisk kalligrafi denne sommeren? Bli med å lær historien bak kinesisk skriftsspråk. Kurset er todelt og varer 3 dager. Vi samles i Løvbladet Café og avslutter med kinesisk film og middag (inkludert i kurset) den siste dagen. Ta med en venn og opplev noe nytt!",
      btnText: "Meld deg på!",
    };
  },
};
</script>

<style lang="scss" scoped>
.home {
  display: flex;
  justify-content: center;
  .wrapper {
    width: fit-content;

    .btn {
      margin-left: auto;
    }
  }
}
</style>
