<template>
<div class="body">
    <v-container>
    <v-row>
      <v-col>
        <v-alert class="mt-8" type="error"
          >La página que busca no existe. Ir a
           <v-btn @click="vistaHome" color="blue darken-4" fab x-small dark>
            <v-icon>mdi-home</v-icon>
          </v-btn>
        </v-alert>
      </v-col>
    </v-row>
  </v-container>
</div>
</template>

<script>
export default {
  name: "notFound-view",
  // props: {},
  data: function () {
    return {};
  },
  // computed: {},
  methods: {
    vistaHome(){
        this.$router.push("/")
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