<template>
  <v-app class="mainV" >
    <v-layout row wrap align-content-start justify-space-between>
      <v-spacer/>
      <v-flex xs12 md6 >
        <v-card class="content">
          <h1>Welcome to ikle.in!</h1>
        </v-card>
      </v-flex>
      
      <v-flex xs12 md6 >
        <v-card class="content">
          <h1>Interesting Things Going on Here..</h1>
        </v-card>
      </v-flex>

      <v-flex xs12 md3 >
        <v-card class="content smalltext">
          This website is a place for my coding projects to live, as well as a place for me to practice and showcase my journey while learning web development.
          Thanks for visiting, and I would love to hear any feedback you have at: <a href="mailto:isaac@ikle.in">isaac@ikle.in</a>
        </v-card>
      </v-flex>

      <v-flex xs12 md6 align-self-start="" class="hidden-sm-and-down">
        <v-img contain class="img1" :src="require('../assets/seattle.jpg')" aspect-ratio="2">

        </v-img>
      </v-flex>

      <v-flex xs12 md3 >
        <v-card class="content smalltext">
          <h5>Current Workstation</h5>
          <ul>
            <li>Dual-boot Windows 10 x64 & Elementary OS 5.1 Hera</li>
            <li>AMD Ryzen 3900x 12-core CPU</li>
            <li>AMD Radeon RX 5700 XT</li>
            <li>32GB Corsair Vengeance RGB Pro RAM</li>
            <li>Sabrent Rocket Pcie 4.0 1TB M.2 SSD</li>
            <li>etc..</li>
            <li>Dual MSI 27" 144hz Curved Monitors</li>
            <li>..and it's STILL cheaper than your Macbook! 😂</li>
          </ul>
        </v-card>
      </v-flex>

      <v-flex xs12 m12>
        <v-card min-height="50" flat class="spacr"></v-card>
      </v-flex>

      <v-spacer/>
    </v-layout>
  </v-app>
</template>

<script>

export default {
  name: 'Home',
  components: {
    
  }
}
</script>

<style>
.mainV {
  padding-top: 1vmax;
  padding-bottom: 1vmax;
  padding-left: 5vw;
  padding-right: 5vw;
  background-color: lightslategrey !important;
  
}
.content {
  margin: 5vmin;
  padding: 5px;
  font-family: Ubuntu;
  text-align: center;
  color: aqua !important;
  background-color: black !important;
}
.smalltext {
  font-size: 150%;
}
.img1 {
  height: auto;
  display: block;
  border-radius: 45% !important;
}
.spacr {
  background-color: lightslategrey !important;
  color: black !important;
}
</style>