<template>
        <v-footer
        color="#102027"
        absolute
        class="font-weight-medium foot"
        dark
      >
        <v-col
          class="text-center"
          cols="12"
        >
        Copyright © {{ new Date().getFullYear() }} - Isaac Klein
        </v-col>
      </v-footer>
</template>

<script>
export default {
  data() {
    return {
      
    }
  }

}
</script>

<style scoped>
.foot {
  font-family: ubuntu;
}
</style>