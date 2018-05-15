<template>
  <div id="app">
    <v-app
      id="inspire"
      dark
    >
      <SideNavAnime></SideNavAnime>
      <TitleBar></TitleBar>
      <v-content>
        <!-- <v-container fluid> -->
          <v-layout wrap fill-height fill-width>
            <!-- <v-flex wrap> -->
              <div class="padding-content">
                <router-view></router-view>
              </div>
            <!-- </v-flex> -->
          </v-layout>
        <!-- </v-container> -->
      </v-content>
    </v-app>
  </div>
</template>

<script>
  import TitleBar from '@/components/TitleBar/TitleBar';
  import SideNavAnime from '@/components/SideNavMenu/SideNavAnime';

  export default {
    components: { SideNavAnime, TitleBar },
  };
</script>

<style lang="scss">
  @import './css/iconfont';
  @import './css/global';

  .padding-content {
    height:100%;
    width: 100%;
    padding: 20px 20px 0px 20px;
  }

</style>