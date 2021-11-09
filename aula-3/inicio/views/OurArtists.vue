<template>
  <div class="artistas">
    <h1>Esta é a página com a listagem de artistas</h1>
  </div>
  <ArtistCard artistName="Tom Walker" artistDescription="O melhor cantor independente / indie, no estilo modern-jazz"/>
  <ArtistCard artistName="Foo Fighters" artistDescription="A banda que as menininhas amam."/>
  <ArtistCard artistName="Edu Falaschi" artistDescription="O melhor vocalista de metal heavy metal / neo-classico do Brasil"/>
</template>

<script>
// @ is an alias to /src

import ArtistCard from "@/components/ArtistCard.vue";

export default {
  name: "Artistas",
  components: {
    ArtistCard,
  },
};
</script>