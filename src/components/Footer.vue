<template>
  <v-footer color="blue darken-4" class="white--text">
    <v-col
      class="text-center"
      cols="12"
    >
      <strong>Bienvenidos a Heroes of the Storm</strong> - {{ new Date().getFullYear() }}
    </v-col>
  </v-footer>
</template>

<script>
export default {
    name: 'footer-component',
    // props: {},
    data: function(){
        return {}
    },
    // computed: {},
    //methods: {}
    // watch: {},
    // components: {},
    // mixins: [],
    // filters: {},
    // -- Lifecycle Methods
    // -- End Lifecycle Methods
}
</script>

<style scoped>
    
</style>