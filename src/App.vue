<template>
  <div>
    <v-toolbar
      app
      dark
      prominent
      image="https://cdn.vuetifyjs.com/images/backgrounds/vbanner.jpg"
    >
    
      <v-app-bar-nav-icon @click="drawer = !drawer"></v-app-bar-nav-icon>
      <Header></Header>
      <v-toolbar-title class="warning">Vuetify</v-toolbar-title>

      <v-spacer></v-spacer>
    
      <v-btn icon>
        <v-icon>mdi-export</v-icon>
      </v-btn>
    </v-toolbar>

    <v-navigation-drawer app v-model="drawer">
      <h3>Menu vertical</h3>
      <header-ru></header-ru>
    </v-navigation-drawer>




  </div>
</template>

<script>
import HeaderRu from "./components/HeaderRu.vue"


export default {
  components: { HeaderRu },
  name:"App",
    data(){
      return {
        drawer:null,
      }
    }
};
</script>
