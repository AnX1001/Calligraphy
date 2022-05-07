<template>
  <div class="home">
    <articleBlock
      :imgSrc="require('../assets/' + paint)"
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
      paint: "paintletters.jpeg",
      heading: "Påmelding",
      paragraph:
        "Påmeldingsfrist er 4.juli og vi har plass til maks 20 personer. Avhenging av interessen så vil vi vurdere å kjøre et ekstra kurs. Men pga. at kurset pleier å fylles opp hver sommer, så anbefaler å tidlig påmelding. Vi holder 3-dagers kurset med fire oppstartsdatoer. Husk å velge den startdato som passer deg best. Vi ses på kurs!",
    };
  },
};
</script>

<style lang="scss" scoped></style>
