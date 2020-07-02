<template>
    <v-app style="appmain background: #ECEDF0;" width="100%" >
        <v-layout column>
            <Header></Header>
            <v-content>
            
            <router-view/>
            
            </v-content>
            <Footer></Footer>
        </v-layout>
    </v-app>
</template>

<script>
import Header from '@/components/Header.vue';
import Footer from '@/components/Footer.vue';

export default {
    name: 'App',

    components: {
        Header
        ,Footer
    },

    data: () => ({
        //
    }),
};
</script>

<style>
.appmain {
    margin: auto;
    align-content: center;
}
</style>
