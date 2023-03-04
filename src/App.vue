<template>
  <div>
    <header-ru></header-ru>

    <v-navigation-drawer app v-model="drawer">
      <h3>Menu vertical</h3>
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
