<template>
  <v-app id="inspire">
    <Drawer :drawer="drawer" @opened="opened"/>

    <v-app-bar app>
      <v-app-bar-nav-icon @click="drawer = !drawer"></v-app-bar-nav-icon>

      <v-toolbar-title>Application</v-toolbar-title>
    </v-app-bar>

    <v-main>
      <HelloWorld/>
    </v-main>
    <Footer/>
  </v-app>
</template>

<script>
import HelloWorld from './components/HelloWorld';
import Footer from './components/Footer';
import Drawer from './components/Drawer';

export default {
  name: 'App',

  components: {
    HelloWorld,
    Footer,
    Drawer,
  },

  data: () => ({
    drawer: null
  }),

  methods: {
    opened(isOpened) {
      this.drawer = isOpened;
      console.log("열림>>>  " + isOpened);
    }
  }
};
</script>
