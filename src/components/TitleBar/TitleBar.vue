<template>
  <v-toolbar
      color="grey darken-4"
      dense
      fixed
      clipped-left
      app
      flat
      class="drag"
    >
      <!-- <v-toolbar-side-icon @click.stop="drawer = !drawer" class="no-drag"></v-toolbar-side-icon> -->
      <v-toolbar-title class="mr-5 align-center">
        <span class="title">Otaku Collection</span>
      </v-toolbar-title>
      <v-spacer></v-spacer>
      <v-layout row justify-end class="clip-right">
        <user style="padding-right:50px"></user>
        <buttons></buttons>
      </v-layout>
    </v-toolbar>
</template>

<script>
  import Buttons from '@/components/TitleBar/Buttons';
  import User from '@/components/TitleBar/User';

  export default {
    components: { User, Buttons },
  };
</script>

<style lang="scss">
  .clip-right{
    margin-right: 0px !important;
  }
</style>

