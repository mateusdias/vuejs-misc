<template>
  <div id="artistbanner" :style="customArtistBackground">
    <div id="artisttitle">
      <h1>{{ name }}</h1>
      <p>{{ description }}</p>
    </div>
    <div id="listen">
      <v-btn class="button">{{buttontext}}</v-btn>
    </div>
  </div>
</template>

<script>
export default {
  name: "ArtistBanner",
  props: {
    name: String,
    description: String,
    cover: String,
    buttontext: String
  },
  computed: {
    customArtistBackground() {
      const imgDinamica = require("@/assets/artists/" + this.cover + ".jpg");
      return (
        "margin: 20px auto; width: 800px; height:376px; background-image: url('" +
        imgDinamica +
        "'); background-repeat: no-repeat;"
      );
    },
  },
};
</script>

<style scoped>
#artisttitle {
  padding: 20px;
  background-color: white;
  opacity: 0.8;
  text-align: center;
}
#artisttitle h1 {
  font-size: 40px;
  margin: 0;
  padding: 0;
}
#artisttitle p {
  font-size: 20px;
  margin: 0;
  padding: 0;
}
.button {
  background-color: #57aa7d;
  border: none;
  color: white;
  padding: 20px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 22px;
  margin: 4px 2px;
  border-radius: 12px;
}
#listen {
  position: relative;
  top: 170px;
}
</style>
