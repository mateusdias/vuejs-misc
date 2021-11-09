<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/vinew.png" />
    <ArtistBanner name="U2" description="A maior banda pop rock de todos os tempos" cover="u2" buttontext="Ouvir"/>
    <ArtistBanner name="Edu Falaschi" description="Vocalista de metal" cover="falaschi" buttontext="Ouça já"/>
    <ArtistBanner name="Metallica" description="Aquela banda que todo mundo conhece a musica Nothing Else Matters" cover="metallica" buttontext="Compre ingressos para o show em SP"/>
  </div>
</template>

<script>
// @ is an alias to /src
import ArtistBanner from "@/components/ArtistBanner.vue";

export default {
  components: {
    ArtistBanner
  },
};
</script>


<style scoped>

</style>