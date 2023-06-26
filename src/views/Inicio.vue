<template>
<div class="body">
  <v-container>
    <v-row>
      <v-col>
        <v-alert outlined color="white" class="text-center mx-auto mt-8" width="31.25rem">
          <div class="text-h6">Desafía las expectativas de los MOBA</div>
          <div>
            Épicos héroes y acción sin cesar en múltiples campos de batalla
          </div>
          <v-btn @click="vistaPersonajes" elevation="2" class="orange darken-3 white--text mt-5"
            >VER HÉROES</v-btn
          >
        </v-alert>
        <v-alert color="purple darken-1" class="text-caption white--text mt-8">
          ¡Te damos la bienvenida al Nexo! ¡En este reino entre reinos, todo es
          posible! Elige entre decenas de héroes legendarios de todo el panteón
          de Blizzard, personaliza sus talentos y habilidades en medio del
          combate y lucha en una infinidad de campos de batalla que redefinen el
          género. ¡Esto no es un MOBA promedio, esto es Heroes of the Storm!
        </v-alert>
      </v-col>
    </v-row>
  </v-container>
</div>
</template>

<script>
export default {
  name: "inicio-view",
  // props: {},
  data: function () {
    return {};
  },
  // computed: {},
  methods: {
    vistaPersonajes(){
       this.$router.push("/personajes")
    }
  }
  // watch: {},
  // components: {},
  // mixins: [],
  // filters: {},
  // -- Lifecycle Methods
  // -- End Lifecycle Methods
};
</script>

<style scoped>
.body{
  background-image: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)),
                     url("https://cdn.wallpapersafari.com/83/37/C6ypOG.jpg");
  background-size: cover;
  height: 100%;
}
</style>