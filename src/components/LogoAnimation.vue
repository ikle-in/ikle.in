<template>
  <v-app>
    <v-card
      flat
      height=auto
      tile
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
        <v-btn to="/home">Home</v-btn>
        <v-btn to="/about">About</v-btn>
        <v-btn to="/projects">Projects</v-btn>
        <v-btn to="/misc">Misc</v-btn>
      </v-navigation-drawer>

    </v-card>

    <v-card height=100% color=#121212 tile>
      <v-card 
      class="ma-16 bg"
      height=60% 
      rounded
      color=#263238
      >
        <v-card 
        class="welcome" 
        style='background: rgb(8,147,237); background: linear-gradient(0deg, rgba(8,147,237,1) 0%, rgba(50,223,137,1) 100%);' 
        height=auto
        
        >
          <p class="text-center" 
          style="color: black"
          >
            Welcome to ikle.in!
          </p>
        </v-card>

        

        <v-card
        height="20%"
        width="90%"
        class="centered"
        style='background: #263238;'
        tile
        flat
        >
          <p 
          class="content"
          style="color: rgba(255,255,255,0.6)"
          >Hello World! My name is Isaac Klein and this website is a place for my coding projects and more. I currently know Java and am 
            getting started with web development. I am currently learning Vue.js, Node.js, JavaScript, and a little HTML and CSS. Stay tuned for updates, and thanks for visiting.
          </p>
        </v-card>

        <v-card
        class="centered largeTxt"
        
        >
          ikle.in
        </v-card>

      </v-card>
    </v-card>


    <v-footer
        color="blue-grey darken-4"
        absolute
        class="font-weight-medium"
        dark
      >
        <v-col
          class="text-center"
          cols="12"
        >
        Copyright © {{ new Date().getFullYear() }} - Isaac Klein
        </v-col>
      </v-footer>


  </v-app>
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

<style>
  .v-card {
    font-family: 'Ubuntu', sans-serif;
    font-style: bold;
  }
  .v-footer {
    font-family: 'Ubuntu', sans-serif;
    font-style: thin;
  }
  .welcome {
    font-size: 30px;
    text-align: center;
    text-shadow: 1px 1px darkgray;
  }
  .centered {
    margin: auto;
  }
  .content {
    min-height: 10vh;
    text-align: center;
    font-size: calc(0.5rem + 0.8vw);
    margin: auto;
  }
  .largeTxt {
    margin-top: 20vh;
    text-align: center;
    font-size: calc(1.5rem + 1.5vw);
    width: 30vw;
    min-width: 30vw;
    animation-name: example;
    animation-duration: 8s;
    animation-iteration-count: infinite;
  }
  @keyframes example {
  0%   {background-color:#ffb3ba; left:0px; top:-10vw;}
  25%  {background-color:#ffdfba; left:10vw; top:0px;}
  50%  {background-color:#ffffba; left:0px; top:10vw;}
  75%  {background-color:#baffc9; left:-10vw; top:0px;}
  100% {background-color:#ffb3ba; left:0px; top:-10vw;}
}
.bg {
    min-height: fit-content;
    max-height: fit-content;
}
.menu_item {
  color: rgba(255, 255, 255, 0.87);
  text-align: center;
  margin: auto;
}


</style>
