<template>
    <v-card
      flat
      tile
      class="head"
    >
      <v-toolbar dense color="blue-grey darken-4" dark>
        <v-app-bar-nav-icon @click.stop="drawer = !drawer" >
        </v-app-bar-nav-icon>
        <v-toolbar-title>ikle.in</v-toolbar-title>
        <v-spacer></v-spacer>
      </v-toolbar>

      <v-navigation-drawer 
      v-model='drawer' 
      app 
      color="#263238" 
      temporary 
      dark
      width="200px"
      >
        
        <v-btn tile to="/" class="menubtn">Home</v-btn>
        <v-btn tile to="/about" class="menubtn">About</v-btn>
        <v-btn tile to="/projects" class="menubtn">Projects</v-btn>
        <v-btn tile to="/misc" class="menubtn">Misc</v-btn>
       

      </v-navigation-drawer>

    </v-card>
</template>

<script>
export default {
  data() {
    return {
      drawer: false
    }
  }

}
</script>

<style scoped>
.head {
    width: 100%;
    height: 48px;
}
.menubtn {
  border: 1px solid black; 
  cursor: pointer; /* Pointer/hand icon */
  display: block; /* Make the buttons appear below each other */
  padding: 7px !important;
  
}
</style>