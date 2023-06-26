<template>
  <div>
    <v-app-bar color="blue darken-4" dark>
      <v-row align="center" justify="space-around">
        <v-btn @click="vistaInicio" tile color="blue darken-3">
          <v-icon left> mdi-home </v-icon>
          Home
        </v-btn>
      </v-row>
    </v-app-bar>
  </div>
</template>

<script>
export default {
  name: "navbar-component",
  // props: {},
  data: function () {
    return {};
  },
  // computed: {},
  methods: {
    vistaInicio(){
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
</style>