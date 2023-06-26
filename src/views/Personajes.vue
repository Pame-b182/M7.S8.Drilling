<template>
<div class="personajes">
    <v-container>
    <v-row justify="center">
      <v-col cols="12" sm="10" class="white--text">
        <div>
          <h1>Héroes</h1>
          <div>
            <v-icon class="icon white--text">mdi-shield</v-icon>
            <v-icon class="icon white--text">mdi-crosshairs-gps</v-icon>
            <v-icon class="icon white--text">mdi-plus</v-icon>
            <v-icon class="icon white--text">mdi-sword</v-icon>
            <v-icon class="icon white--text">mdi-human-child</v-icon>
            <v-icon class="icon white--text">mdi-cursor-pointer</v-icon>
          </div>
        </div>
        <v-simple-table dark class="table mt-5">
          <template v-slot:default>
            <thead>
              <tr>
                <th class="text-center">Héroe</th>
                <th class="text-center">Nombre</th>
                <th class="text-center">Función</th>
                <th class="text-center">Título</th>
                <th class="text-center">Ataque</th>
              </tr>
            </thead>
            <tbody>
              <tr v-for="heroe in heroes" :key="heroe.nombre">
                <td>
                  <v-img
                    contain
                    max-height="170"
                    max-width="170"
                    :src="heroe.imagen"
                  ></v-img>
                </td>
                <td class="text-center">{{ heroe.nombre }}</td>
                <td class="text-center">{{ heroe.funcion }}</td>
                <td class="text-center">{{ heroe.titulo }}</td>
                <td class="text-center">{{ heroe.ataque }}</td>
              </tr>
            </tbody>
          </template>
        </v-simple-table>
      </v-col>
    </v-row>
  </v-container>
</div>
</template>

<script>
import {mapState} from 'vuex'
export default {
  name: "personajes-view",
  // props: {},
  data: function () {
    return {
    };
  },
  computed: {
    ...mapState(['heroes'])
  },
  //methods: {}
  // watch: {},
  // components: {},
  // mixins: [],
  // filters: {},
  // -- Lifecycle Methods
  // -- End Lifecycle Methods
};
</script>

<style scoped>
.icon{
  padding: 0 8px;
  font-size: 30px;
}
.table{
  max-height: 70vh;
  overflow: auto;
}
.personajes {
  background-image: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)),
    url("https://wallpapercrafter.com/desktop1/555898-heroes-of-the-storm-Sylvanas-Windrunner-contests.jpg");
  background-size: cover;
}
</style>